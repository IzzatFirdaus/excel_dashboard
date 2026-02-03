# CADANGAN TEKNIKAL: PEMBANGUNAN SISTEM INTEGRASI DATA DAN PAPAN PEMUKA PRESTASI

**Status Dokumen:** Draf Perancangan Awal
**Klasifikasi:** Terbuka (Sehingga data sebenar dimasukkan)

---

## 1.0 RINGKASAN EKSEKUTIF

Dokumen ini memperincikan cadangan teknikal bagi pembangunan platform integrasi data yang memproses fail hamparan elektronik (*Excel*) kepada visualisasi papan pemuka (*Dashboard*). Sistem ini bertujuan untuk mengautomasikan penerimaan data, melaksanakan pengesahan (*validation*), menormalkan struktur data, dan memaparkan analitik menerusi antara muka pengguna atau alat risikan perniagaan (*Business Intelligence*).

Cadangan ini menggariskan tiga model seni bina berbeza—skala kecil, ETL berjadual, dan pemprosesan masa nyata—untuk dipilih berdasarkan keperluan agensi dan infrastruktur sedia ada.

---

## 2.0 OBJEKTIF DAN BATASAN PELAKSANAAN

### 2.1 Objektif

1. Menyediakan mekanisme pemusatan data daripada pelbagai fail sumber (*Excel*) ke dalam satu pangkalan data berstruktur.
2. Memastikan integriti data melalui proses pengesahan dan sanitasi input yang ketat.
3. Menghasilkan pelaporan visual yang dinamik bagi menyokong proses pembuatan keputusan.

### 2.2 Batasan dan Keperluan Teknikal

* **Persekitaran Operasi:** Sistem perlu beroperasi secara optimum di persekitaran Windows menggunakan pelayan web Laragon (penggunaan *Docker* adalah opsyenal).
* **Mod Input:** Menyokong muat naik manual dan integrasi aliran kerja automatik (jika perlu).
* **Keselamatan:** Pematuhan kepada garis panduan keselamatan siber, termasuk pencegahan suntikan formula (*formula injection*) dan kawalan akses.

---

## 3.0 MODEL SENI BINA SISTEM (OPSYEN PELAKSANAAN)

Pihak pengurusan perlu memilih satu daripada tiga opsyen berikut berdasarkan skala operasi:

### Opsyen A: Model Pemprosesan Setempat (Kompleksiti Rendah)

* **Deskripsi:** Pengguna memuat naik fail, pelayan memproses data secara langsung ke format JSON, dan paparan visual dijana pada pelayar pengguna.
* **Kesesuaian:** Pasukan kecil, pelaporan *ad-hoc*, dan saiz fail yang kecil (< 10MB).
* **Stack Teknologi:** *Backend* (Laravel/Node/Python), Pustaka Excel (`phpspreadsheet`/`pandas`), *Frontend* (React/Vue + Chart.js).

### Opsyen B: Model ETL Berjadual & Gudang Data (Kompleksiti Sederhana)

* **Deskripsi:** Fail dimuat naik ke zon penampan (*staging area*). Proses ETL (*Extract, Transform, Load*) berjadual akan menormalkan data ke dalam pangkalan data berelasi.
* **Kesesuaian:** Pelaporan berkala, fail bersaiz besar, pelbagai templat, dan keperluan audit data sejarah.
* **Stack Teknologi:** Penjadual Tugas (*Task Scheduler/Cron*), Pangkalan Data (MySQL/PostgreSQL).

### Opsyen C: Model Pemprosesan Masa Nyata (Kompleksiti Tinggi)

* **Deskripsi:** Pemprosesan latar belakang menggunakan barisan giliran (*queue*) dan pekerja (*workers*). Kemaskini dihantar ke papan pemuka menggunakan teknologi *WebSocket*.
* **Kesesuaian:** Jumlah transaksi tinggi, ramai pengguna serentak, dan keperluan data masa nyata.
* **Stack Teknologi:** Pengurusan Giliran (Redis + Bull/Celery), *Streaming Parser*.

---

## 3.X PERANCANGAN KHUSUS: LARAVEL 12

Seksien ini menerangkan garis panduan pelaksanaan menggunakan **Laravel 12** sebagai rangka kerja backend utama. Ia merangkumi pakej disyorkan, struktur projek, kawalan keselamatan, strategi pekerja/antrian, penyebaran pada Laragon (Windows) dan pilihan Docker.

### 3.X.1 Rasional Pemilihan

* Laravel 12 menawarkan ekosistem matang (Eloquent, Queues, Scheduler), sokongan komuniti, dan kemudahan integrasi dengan servis seperti Redis, Horizon, dan Sentry. Sesuai untuk pembangunan pantas sambil mengekalkan piawaian keselamatan.

### 3.X.2 Pakej & Perpustakaan Disyorkan

* `maatwebsite/excel` atau `box/spout` untuk baca/tulis Excel.
* `spatie/laravel-permission` untuk RBAC.
* `spatie/laravel-activitylog` untuk jejak audit.
* `laravel/horizon` untuk pemantauan queue (Redis).
* `laravel/sanctum` atau `passport` untuk auth API jika perlu.
* `sentry/sentry-laravel` untuk error tracking.

### 3.X.3 Skop Modul Teras

* `app/Imports` — logik parsing Excel dan pemetaan schema.
* `app/Jobs` — pekerjaan latar (parsing, transform, aggregate).
* `app/Services/ExcelParser` — servis bersih untuk transformasi dan sanitasi.
* `routes/api.php` — endpoint muat naik dan status.
* `storage/app/uploads_secure` — lokasi simpanan fail mentah di luar public webroot.

### 3.X.4 Konfigurasi & Persekitaran

* Simpan konfigurasi sensitif dalam `.env` (DB, Redis, SENTRY_DSN, STORAGE_DRIVER).
* Tetapkan had muat naik (`upload_max_filesize`, `post_max_size`) dan had baris/ lajur di parser.
* Gunakan env `APP_ENV` dan profil staging/production.

### 3.X.5 Strategi Queue & Penjadualan

* Gunakan Redis sebagai driver queue; laravel-horizon untuk pemantauan dan retry toolbox.
* Jalankan `php artisan schedule:run` melalui Windows Task Scheduler pada Laragon; jika Docker digunakan, gunakan `cron` container atau `scheduler` service.
* Implement dead-letter queue pattern dan metrics untuk tugas yang gagal.

### 3.X.6 Pematuhan Keselamatan

* Validasi MIME + ekstensi, imbas antivirus (Windows Defender / ClamAV) sebelum parsing.
* Escape sel bermula dengan `=,+,-,@` dan tidak evaluate formula dalam proses.
* Terapkan RBAC (`spatie/permission`), rate limiting dan logging akses.
* Audit trail untuk setiap muat naik, proses ETL, dan kemaskini data.

### 3.X.7 Ujian & Standard KualITI

* Unit tests (`phpunit`/Pest) untuk parser, transform dan job behaviour.
* Integration tests untuk aliran upload→queue→worker→DB.
* Gunakan `phpcs`/`phpstan` dan `php-cs-fixer` dalam CI untuk standard kod.

### 3.X.8 Migrasi & Naik Taraf

* Jika naik taraf dari versi Laravel terdahulu, semak `upgrade guide` rasmi dan dependensi PHP (versi minimum PHP yang disokong oleh Laravel 12). Rancang migrasi database dan backlog untuk breaking changes.

### 3.X.9 Fail & Perubahan yang Dicadangkan

* `routes/api.php` — endpoint `/upload` dan `/upload/status`.
* `app/Imports/ExcelImport.php` — pengeksport dan parser.
* `app/Jobs/ProcessUpload.php` — job utama untuk parsing & transform.
* `database/migrations/*` — jadual `files`, `rows`, `datasets`, `metrics`.
* `docker-compose.yml` (optional) — Redis, Postgres, MinIO, dan horizon worker.

### 3.X.10 Checklist Penyebaran (Laragon / Docker)

* Pastikan PHP & extensi (ext-gd, ext-zip) memenuhi keperluan Laravel 12.
* Konfigurasi `worker` (supervisor/Horizon) dan jadual `schedule` (Task Scheduler / cron).
* Konfigurasi backup DB dan storan, serta pemantauan (Sentry, Prometheus/Grafana).

---

## 4.0 TADBIR URUS DATA DAN PENGESAHAN

### 4.1 Pemodelan Data

* **Penyimpanan:** Menyimpan fail sumber asal (mentah) dan data kanonik yang telah dinormalisasi (*row-oriented*).
* **Struktur:** Setiap rekod perlu mengandungi metadata seperti `source_file_id`, `sheet_name`, `row_number`, dan cap masa.

### 4.2 Mekanisme Pengesahan (Data Validation)

Sistem mesti mematuhi logik perniagaan berikut sebelum data disimpan:

1. **Format Fail:** Memastikan format MIME dan ekstensi fail adalah sah.
2. **Integriti Struktur:** Semakan kehadiran *header*, konsistensi lajur, dan format data (tarikh/nombor).
3. **Sanitasi:** Pencegahan serangan siber melalui input fail.

---

## 5.0 KAWALAN KESELAMATAN (PEMATUHAN KRISA/PPrISA)

Pembangunan sistem perlu mematuhi prinsip **Kerahsiaan, Integriti, dan Ketersediaan (CIA Triad)**:

1. **Sanitasi Input:** Semua sel Excel yang bermula dengan simbol `=, +, -, @` mesti dinyaaktifkan (*escaped*) bagi mengelakkan serangan *CSV/Formula Injection*.
2. **Imbasan Hasad:** Integrasi dengan perisian antivirus (contoh: Windows Defender CLI) untuk mengimbas fail sebelum pemprosesan.
3. **Kawalan Akses (RBAC):** Pelaksanaan kawalan akses berasaskan peranan bagi fungsi muat naik dan paparan papan pemuka.
4. **Jejak Audit (Audit Trail):** Merekodkan log aktiviti bagi setiap muat naik, pemprosesan, dan ralat sistem.

---

## 6.0 PENGURUSAN PRESTASI DAN PENYELENGGARAAN

* **Pengendalian Fail Besar:** Menggunakan teknik *chunking* atau *streaming* bagi mengelakkan kegagalan memori (*memory exhaustion*).
* **Strategi Penimbalan (Caching):** Menggunakan Redis untuk menyimpan hasil agregat bagi mengurangkan beban pangkalan data.
* **Penyebaran (Deployment):**
* Jika menggunakan Laragon: Menggunakan *Windows Task Scheduler* untuk proses latar belakang.
* Jika menggunakan Docker (Disyorkan): Menggunakan kontena berasingan untuk pelayan web, pangkalan data, dan pekerja giliran (*queue workers*).

---

## 7.0 HALA TUJU DAN TINDAKAN LANJUT

Bagi memulakan fasa pembangunan, keputusan berikut diperlukan:

1. **Pemilihan Platform:** Menentukan penggunaan bahasa pengaturcaraan (PHP/Laravel, Node.js, atau Python).
2. **Analisis Keperluan:** Menakrifkan profil fail (saiz, kekerapan) dan templat data yang terlibat.
3. **Pemilihan Model:** Memilih Opsyen A, B, atau C berdasarkan sumber manusia dan infrastruktur.
4. **Spesifikasi Antara Muka:** Membangunkan prototaip papan pemuka dan skema pangkalan data.

---

### Lampiran: Cadangan Struktur Direktori Projek

Bagi memastikan kod sumber mudah diselenggara, struktur berikut dicadangkan (Contoh berasaskan Laravel):

* `app/Imports`: Logik penguraian (*parsing*) Excel.
* `app/Jobs`: Tugas latar belakang (*Queued Jobs*).
* `app/Services/DataProcessing`: Logik perniagaan untuk pengesahan dan sanitasi.
* `storage/app/uploads_secure`: Lokasi penyimpanan fail mentah (di luar *public webroot*).
* `resources/lang/ms`: Fail lokalisasi Bahasa Melayu bagi antara muka pengguna.
* `docs/`: Dokumentasi teknikal dan manual pengguna.

> **Nota Pematuhan Bahasa:** Dokumentasi sistem dan antara muka pengguna (UI) hendaklah diutamakan dalam **Bahasa Melayu**, manakala kod sumber dan komen teknikal dikekalkan dalam Bahasa Inggeris bagi tujuan piawaian antarabangsa.
