# SPESIFIKASI KEPERLUAN PERISIAN (SRS) & CADANGAN TEKNIKAL

## SISTEM INTEGRASI DATA DAN PAPAN PEMUKA PRESTASI NASIONAL (National Integrated Performance Monitor)

| Butiran Dokumen | Keterangan |
|---|---|
| **Tajuk Projek** | Sistem Integrasi Data dan Papan Pemuka Prestasi Nasional |
| **Versi Dokumen** | 2.0 |
| **Status** | Cadangan Teknikal Rasmi (Untuk Kelulusan Jawatankuasa Pemandu) |
| **Klasifikasi** | TERHAD — Untuk Edaran Dalaman Sahaja |
| **Tarikh Kemaskini** | 10 Februari 2026 |
| **Pematuhan** | KRISA (Kerangka Rujukan Keselamatan ICT Sektor Awam), PPrISA (Polisi Penggunaan dan Keselamatan ICT Sektor Awam), NCII (National Critical Information Infrastructure) |
| **Disediakan Oleh** | Unit HEAD, Kementerian Pendidikan Tinggi (KPT) |

---

## 1.0 RINGKASAN EKSEKUTIF

### 1.1 Latar Belakang

Pada masa kini, pemantauan prestasi merentas jabatan dan agensi di bawah portfolio Kerajaan Malaysia masih bergantung kepada proses manual yang tidak seragam. Data prestasi dikumpul melalui pelbagai fail hamparan elektronik (Microsoft Excel) yang diedar secara emel, disimpan dalam storan tempatan (local storage) tanpa kawalan versi, dan dianalisis secara ad hoc tanpa mekanisme pengesahan data yang konsisten. Amalan ini menimbulkan risiko kritikal terhadap integriti data, ketepatan pelaporan, dan kebolehauditan proses tadbir urus.

### 1.2 Justifikasi Projek

Cadangan ini mencadangkan pembangunan sebuah platform bersepadu dikenali sebagai **National Integrated Performance Monitor** — sebuah repositori pusat (Centralized Data Repository) yang menyatukan seluruh data prestasi daripada pelbagai jabatan, agensi, dan program strategik ke dalam satu ekosistem digital yang terkawal. Sistem ini akan menggantikan sepenuhnya proses legasi semasa melalui:

* **Automasi Pengumpulan Data** — Penggantian proses emel dan pengumpulan manual kepada muat naik pukal (Bulk Upload) melalui antara muka web yang terkawal.
* **Pengesahan Data Berlapis** — Setiap data yang diterima akan melalui proses pengesahan struktur (Structural Validation), pengesahan format (Format Validation), dan sanitasi keselamatan (Security Sanitization) sebelum dimasukkan ke dalam pangkalan data produksi.
* **Papan Pemuka Analitik Masa Nyata** — Pemantauan prestasi secara visual dan interaktif yang menyokong proses membuat keputusan berasaskan data (Data-Driven Decision Making).
* **Jejak Audit Lengkap** — Pematuhan KRISA, PPrISA, dan NCII melalui pencatatan setiap transaksi data yang boleh diaudit.

### 1.3 Hasil Jangkaan

Sistem ini dijangka meningkatkan kecekapan pelaporan prestasi sebanyak sekurang-kurangnya 60%, mengurangkan ralat data manual, memperkukuh ketelusan tadbir urus, dan menyediakan asas analitik ramalan (Predictive Analytics) bagi menyokong penilaian risiko dan tindakan pembetulan proaktif di peringkat strategik nasional.

---

## 2.0 OBJEKTIF PROJEK

Objektif strategik projek ini adalah seperti berikut:

| No. | Objektif | Petunjuk Pencapaian (Outcome Indicator) |
|---|---|---|
| **OBJ-01** | Mewujudkan repositori data terpusat (Centralized Data Repository) yang menyatukan semua rekod prestasi daripada pelbagai sumber hamparan elektronik ke dalam satu pangkalan data relasi yang terurus dan terkawal. | Satu pangkalan data tunggal menggantikan semua fail Excel silo. |
| **OBJ-02** | Menjamin integriti dan ketepatan data melalui automasi pengesahan berlapis (Multi-Layer Validation), sanitasi input keselamatan (Security Sanitization), dan mekanisme kelulusan data (Approval Workflow) sebelum data diiktiraf sebagai data produksi. | Kadar ralat data kurang daripada 2% selepas pengesahan automatik. |
| **OBJ-03** | Menyokong pemantauan prestasi masa nyata (Real-Time Performance Monitoring) melalui papan pemuka analitik (Analytics Dashboard) yang memaparkan status KPI, pencapaian mengikut jabatan, dan analisis perbandingan (Benchmarking) secara dinamik. | Papan pemuka boleh diakses dalam masa kurang daripada 3 saat. |
| **OBJ-04** | Memudahkan pengurusan kitaran hayat KPI (KPI Lifecycle Management) — daripada pendaftaran teras strategik, penetapan sasaran, kemasukan data berkala, hinggalah analisis pencapaian — secara berstruktur, berjadual, dan boleh diaudit. | Jejak audit lengkap bagi setiap perubahan KPI. |
| **OBJ-05** | Menyediakan keupayaan analitik ramalan (Predictive Analytics) termasuk unjuran prestasi KPI (KPI Forecasting), pemarkahan risiko automatik (Automated Risk Scoring), dan pengesanan anomali data (Anomaly Detection) bagi menyokong tindakan pembetulan proaktif. | Model ramalan mencapai ketepatan minimum 80%. |

---

## 3.0 SKOP PEMBANGUNAN SISTEM (TERPERINCI)

Skop pembangunan merangkumi sembilan (9) modul teras yang direka bentuk secara modular dan berintegrasi. Setiap modul diterangkan secara terperinci dari segi fungsi, keperluan fungsian, dan aliran logik.

---

### 3.1 Modul Pengurusan Pengguna dan Kawalan Akses (User Management & Access Control Module)

**Tujuan:** Mengawal identiti, peranan, dan kebenaran setiap pengguna sistem bagi menjamin keselamatan akses dan kebolehauditan.

#### 3.1.1 Kawalan Akses Berasaskan Peranan (Role-Based Access Control, RBAC)

Sistem melaksanakan model RBAC bertingkat dengan peranan berikut:

| Peranan (Role) | Hak Akses Utama |
|---|---|
| **Pentadbir Sistem** (Super Admin) | Pengurusan penuh: pengguna, peranan, konfigurasi sistem, dan jejak audit. |
| **Pentadbir Jabatan** (Department Admin) | Pengurusan pengguna dan data dalam skop jabatan ditugaskan. |
| **Pengurus KPI** (KPI Manager) | Pendaftaran KPI, penetapan sasaran, kelulusan data, dan semakan laporan. |
| **Pengendali Data** (Data Operator) | Kemasukan data manual dan muat naik fail Excel. |
| **Pemerhati** (Viewer) | Akses baca sahaja (Read-Only) kepada papan pemuka dan laporan. |
| **Juruaudit** (Auditor) | Akses kepada jejak audit dan laporan pematuhan. |

#### 3.1.2 Pengesahan Identiti (Authentication)

* Pengesahan kata laluan (Password Authentication) dengan polisi kekuatan kata laluan minimum (sekurang-kurangnya 12 aksara, gabungan huruf besar, huruf kecil, nombor, dan aksara khas).
* Pengesahan Dua Faktor (Two-Factor Authentication, 2FA) melalui kod OTP (One-Time Password) yang dihantar ke emel berdaftar atau aplikasi pengesah (Authenticator App).
* Mekanisme kunci akaun automatik (Account Lockout) selepas lima (5) percubaan log masuk gagal berturut-turut.

#### 3.1.3 Log Aktiviti Pengguna (User Activity Log)

Setiap tindakan kritikal oleh pengguna direkod secara automatik, termasuk:

* Log masuk dan log keluar (Login/Logout).
* Muat naik fail, kemaskini data, dan pemadaman rekod.
* Kelulusan atau penolakan data.
* Eksport laporan dan muat turun data.
* Perubahan peranan atau kebenaran pengguna.

Setiap entri log mengandungi: identiti pengguna, cap masa (Timestamp), jenis tindakan, alamat IP, dan kesan perubahan (Change Delta).

---

### 3.2 Modul Pengurusan Strategi dan KPI (Strategy & KPI Management Module)

**Tujuan:** Menyediakan struktur hierarki bagi pendaftaran dan pengurusan kitaran hayat KPI, daripada peringkat teras strategik sehinggalah petunjuk prestasi operasi.

#### 3.2.1 Hierarki Strategik

Sistem menyokong empat (4) peringkat hierarki strategik:

| Peringkat | Keterangan | Contoh |
|---|---|---|
| **Teras Strategik** (Strategic Core) | Matlamat induk organisasi atau negara. | "Memantapkan Modal Insan" |
| **Strategi** (Strategy) | Hala tuju pelaksanaan bagi setiap teras. | "Meningkatkan kualiti pendidikan tinggi" |
| **Inisiatif** (Initiative) | Program atau projek khusus bagi melaksanakan strategi. | "Program Pengantarabangsaan Universiti Awam" |
| **KPI** (Key Performance Indicator) | Petunjuk prestasi terukur bagi setiap inisiatif. | "Peratus graduan mendapat pekerjaan dalam 6 bulan" |

#### 3.2.2 Pengurusan Versi KPI (KPI Versioning)

* Setiap perubahan terhadap definisi KPI, formula pengiraan, atau sasaran tahunan akan menghasilkan versi baharu (New Version) tanpa memadamkan versi terdahulu.
* Sejarah versi (Version History) dikekalkan sepenuhnya bagi membolehkan perbandingan merentas tempoh pelaporan dan audit retrospektif.
* Setiap peralihan versi memerlukan kelulusan daripada Pengurus KPI dan direkod dalam jejak audit.

#### 3.2.3 Pemetaan KPI

* KPI dipetakan kepada jabatan pelaksana, program induk, dan tempoh pelaporan (suku tahun / tahunan).
* Sokongan KPI bersilang jabatan (Cross-Departmental KPI) yang memerlukan data daripada lebih satu sumber.
* Penetapan pemberat (Weighting) bagi setiap KPI untuk pengiraan skor komposit prestasi jabatan.

---

### 3.3 Modul Kemasukan Data (Data Entry Module)

**Tujuan:** Menyediakan mekanisme kemasukan data yang fleksibel, selamat, dan boleh diaudit melalui dua kaedah: borang dinamik (Dynamic Forms) dan muat naik pukal (Bulk Upload) melalui fail Excel.

#### 3.3.1 Kaedah Kemasukan Data

**A. Borang Dinamik (Dynamic Forms)**

* Borang kemasukan data yang dijana secara automatik berdasarkan definisi KPI yang didaftarkan.
* Jenis medan (Field Types) yang disokong: teks, nombor, tarikh, peratusan, senarai pilihan (Dropdown), dan lampiran fail.
* Pengesahan medan masa nyata (Real-Time Field Validation) untuk memastikan konsistensi input.

**B. Muat Naik Pukal melalui Excel (Bulk Upload via Excel)**

* Pengguna memuat naik fail Excel (.xlsx / .xls) melalui antara muka muat naik yang terkawal.
* Sistem menyediakan templat Excel piawai (Standardized Excel Template) yang boleh dimuat turun untuk setiap jenis KPI.
* Had saiz fail maksimum: 10MB per fail muat naik.
* Pemprosesan fail dilaksanakan secara tak segerak (Asynchronous Processing) melalui baris gilir kerja (Job Queue) menggunakan Redis.

#### 3.3.2 Aliran Data: Jadual Penampan ke Jadual Produksi (Staging-to-Production Data Flow)

Proses kemasukan data melalui lima (5) peringkat kawalan yang ketat:

**Peringkat 1 — Penerimaan dan Simpanan Sementara (Ingestion & Staging)**

* Fail Excel yang dimuat naik disimpan dalam storan sementara (Temporary Storage) dengan pencatatan metadata: nama fail asal, saiz fail, identiti pengguna, dan cap masa muat naik.
* Data diekstrak baris demi baris dan dimasukkan ke dalam **Jadual Penampan** (Staging Table) dengan status awal `DRAFT`.
* Fail asal dikekalkan sebagai rujukan audit.

**Peringkat 2 — Pengesahan Struktur (Structural Validation)**

* Pengesahan kewujudan pengepala lajur (Column Headers) yang diperlukan berdasarkan templat piawai.
* Pengesahan konsistensi bilangan lajur bagi setiap baris data.
* Pengesanan baris kosong, baris duplikasi, atau baris tidak lengkap.
* Rekod yang gagal pengesahan struktur ditandakan dengan status `STRUCTURE_ERROR`.

**Peringkat 3 — Pengesahan Format dan Logik (Format & Logic Validation)**

* Pengesahan jenis data: nombor, tarikh (format ISO 8601), peratusan, dan teks.
* Pengesahan julat nilai (Range Validation): contohnya peratusan mestilah antara 0 dan 100.
* Pengesahan rujukan silang (Cross-Reference Validation): kod jabatan, kod KPI mestilah wujud dalam jadual rujukan.
* Sanitasi keselamatan (Security Sanitization): pengesanan dan penyingkiran formula berbahaya (Formula Injection Prevention) seperti sel yang bermula dengan aksara `=`, `+`, `-`, `@`, `\t`, atau `\r`.
* Rekod yang gagal ditandakan dengan status `VALIDATION_ERROR` berserta mesej ralat yang spesifik.

**Peringkat 4 — Semakan dan Kelulusan Pengguna (User Review & Approval)**

* Data yang lulus pengesahan automatik ditandakan dengan status `PENDING_APPROVAL`.
* Pengurus KPI menyemak ringkasan data melalui antara muka semakan (Review Interface) yang memaparkan: jumlah rekod, rekod sah, rekod ralat, dan pratonton data.
* Pengurus KPI boleh meluluskan (Approve), menolak (Reject), atau meminta pembetulan (Request Correction) bagi setiap kumpulan data (Batch).
* Keputusan kelulusan direkod dalam jejak audit.

**Peringkat 5 — Pemindahan ke Jadual Produksi (Production Promotion)**

* Rekod yang diluluskan dipindahkan daripada Jadual Penampan ke **Jadual Produksi** (Production Table) dengan status `APPROVED`.
* Rekod dalam Jadual Penampan dikemaskini kepada status `PROMOTED` dan dikekalkan selama tempoh pengekalan data (Data Retention Period) yang ditetapkan.
* Data dalam Jadual Produksi menjadi sumber tunggal kebenaran (Single Source of Truth) bagi papan pemuka analitik.

#### 3.3.3 Pengurusan Ralat dan Pembetulan (Error Handling & Correction)

* Rekod ralat dipaparkan dalam senarai terperinci dengan: nombor baris asal dalam fail Excel, nama lajur, nilai yang dimasukkan, jenis ralat, dan mesej ralat.
* Pengguna boleh membetulkan rekod ralat secara langsung melalui antara muka pembetulan (Inline Correction) atau memuat naik semula fail yang telah diperbetulkan.
* Sejarah pembetulan direkod sepenuhnya dalam jejak audit.

---

### 3.4 Modul Analitik dan Papan Pemuka (Analytics & Dashboard Module)

**Tujuan:** Menyediakan visualisasi interaktif dan analisis perbandingan (Benchmarking) bagi menyokong pemantauan prestasi secara masa nyata.

#### 3.4.1 Komponen Papan Pemuka (Dashboard Components)

Papan pemuka dibina menggunakan komponen *widget* interaktif FilamentPHP:

| Komponen | Fungsi |
|---|---|
| **Kad Statistik** (Stat Card) | Paparan ringkas angka prestasi utama: jumlah KPI, peratusan pencapaian, bilangan jabatan aktif. |
| **Carta Bar dan Carta Garis** (Bar & Line Charts) | Perbandingan prestasi mengikut tempoh (suku tahun, tahunan) dan mengikut jabatan. |
| **Carta Pai** (Pie Chart) | Taburan status KPI: Tercapai (On Track), Berisiko (At Risk), Tidak Tercapai (Off Track). |
| **Jadual Interaktif** (Interactive Table) | Senarai KPI terperinci dengan fungsi carian, turutan (Sorting), dan penapisan (Filtering). |
| **Peta Haba** (Heat Map) | Visualisasi prestasi mengikut jabatan dan sektor secara serentak. |
| **Penunjuk Tolok** (Gauge Indicator) | Paparan peratusan pencapaian keseluruhan berbanding sasaran. |

#### 3.4.2 Fungsi Penapisan dan Perbandingan (Filtering & Benchmarking)

* **Penapis Utama:** Tahun pelaporan, Suku tahun, Jabatan/Agensi, Sektor, Teras strategik, dan Status KPI.
* **Perbandingan Merentas Jabatan:** Paparan perbandingan prestasi antara jabatan bagi KPI yang sama atau setaraf.
* **Perbandingan Merentas Tempoh:** Analisis trend prestasi KPI bagi tempoh tiga (3) hingga lima (5) tahun ke belakang.
* Semua paparan papan pemuka menyokong eksport dalam format PDF dan Excel.

---

### 3.5 Modul Kecerdasan Buatan dan Analitik Ramalan (AI & Predictive Analytics Module)

**Tujuan:** Menyediakan keupayaan analisis lanjutan yang melampaui pelaporan deskriptif, termasuk unjuran prestasi masa hadapan, pemarkahan risiko automatik, dan pengesanan anomali data.

#### 3.5.1 Unjuran Prestasi KPI (KPI Forecasting)

* **Kaedah:** Penggunaan model statistik siri masa (Time Series Statistical Models) seperti ARIMA (AutoRegressive Integrated Moving Average) dan/atau Exponential Smoothing bagi mengunjurkan nilai KPI suku tahun seterusnya berdasarkan data historikal.
* **Input Data:** Minimum dua belas (12) titik data historikal (contoh: 12 suku tahun atau 3 tahun data).
* **Output:** Nilai unjuran KPI dengan selang keyakinan (Confidence Interval) pada tahap 80% dan 95%.
* **Paparan:** Carta garis unjuran (Forecast Line Chart) yang memaparkan data sebenar berbanding data ramalan dengan jalur ketidakpastian (Uncertainty Band).
* **Kekangan:** Unjuran bersifat panduan strategik dan bukan pengganti analisis pakar domain. Ketepatan model bergantung kepada kualiti dan kuantiti data historikal.

#### 3.5.2 Pemarkahan Risiko Automatik (Automated Risk Scoring)

* **Kaedah:** Pengiraan skor risiko komposit bagi setiap KPI berdasarkan empat (4) faktor:

| Faktor Risiko | Pemberat | Keterangan |
|---|---|---|
| Sisihan daripada Sasaran (Deviation from Target) | 40% | Perbezaan antara pencapaian semasa dan sasaran yang ditetapkan. |
| Trend Prestasi (Performance Trend) | 25% | Arah aliran prestasi tiga suku tahun terakhir: menaik, mendatar, atau menurun. |
| Volatiliti Data (Data Volatility) | 20% | Kestabilan data — sisihan piawai (Standard Deviation) nilai KPI merentas tempoh pelaporan. |
| Tempoh Baki (Time Remaining) | 15% | Baki masa sebelum tarikh akhir pelaporan KPI. |

* **Output:** Skor risiko antara 0 (Risiko Rendah) hingga 100 (Risiko Kritikal) dengan pengkelasan warna:
  * **Hijau** (0–30): Dalam Sasaran (On Track)
  * **Kuning** (31–60): Memerlukan Perhatian (At Risk)
  * **Merah** (61–100): Kritikal — Tindakan Segera Diperlukan (Critical)

* **Tindakan Automatik:** KPI yang mencapai skor risiko melebihi 60 akan mencetuskan notifikasi automatik kepada Pengurus KPI dan Pentadbir Jabatan.

#### 3.5.3 Pengesanan Anomali Data (Data Anomaly Detection)

* **Titik Pelaksanaan:** Pengesanan anomali dilaksanakan semasa proses pengesahan data di Peringkat 3 (Format & Logic Validation) dalam aliran Jadual Penampan.
* **Kaedah:** Pengesanan data luar julat (Outlier Detection) menggunakan kaedah statistik:
  * Julat Antara Kuartil (Interquartile Range, IQR): Nilai di luar 1.5 × IQR ditandakan sebagai anomali.
  * Skor-Z (Z-Score): Nilai dengan skor-Z melebihi ±3 ditandakan sebagai anomali.
* **Respons Sistem:** Rekod yang dikesan sebagai anomali ditandakan dengan amaran (Warning Flag) tetapi tidak ditolak secara automatik. Pengurus KPI menyemak dan membuat keputusan sama ada menerima atau menolak rekod tersebut.
* **Pembelajaran:** Model pengesanan anomali boleh ditala semula (Re-calibrated) oleh Pentadbir Sistem berdasarkan maklum balas pengguna dan perubahan corak data.

---

### 3.6 Modul Pemantauan Audit (Audit Monitoring Module)

**Tujuan:** Menyediakan jejak audit (Audit Trail) yang lengkap, tidak boleh diubah suai (Immutable), dan boleh diakses oleh pihak berkuasa yang berkenaan bagi pematuhan KRISA, PPrISA, dan NCII.

#### 3.6.1 Skop Jejak Audit

Setiap transaksi berikut direkod secara automatik tanpa pengecualian:

* Pengurusan pengguna: pendaftaran, kemaskini peranan, pengaktifan, penyahaktifan.
* Kemasukan data: muat naik fail, kemasukan borang, pembetulan rekod.
* Kelulusan data: kelulusan, penolakan, permintaan pembetulan.
* Akses papan pemuka: paparan laporan, eksport data.
* Pengurusan KPI: pendaftaran, kemaskini, perubahan versi.
* Konfigurasi sistem: perubahan tetapan, pengurusan peranan.

#### 3.6.2 Atribut Entri Audit

Setiap entri jejak audit mengandungi maklumat berikut:

| Atribut | Keterangan |
|---|---|
| ID Audit (Audit ID) | Pengecam unik bagi setiap entri audit. |
| Cap Masa (Timestamp) | Tarikh dan masa tindakan dilaksanakan (format ISO 8601 dengan zon masa). |
| Identiti Pengguna (User Identity) | Nama pengguna, ID pengguna, dan peranan semasa. |
| Alamat IP (IP Address) | Alamat IP sumber tindakan. |
| Jenis Tindakan (Action Type) | Kategori tindakan: CREATE, READ, UPDATE, DELETE, APPROVE, REJECT, EXPORT. |
| Entiti Sasaran (Target Entity) | Jadual, rekod, atau modul yang terkesan. |
| Nilai Sebelum (Before Value) | Nilai data sebelum perubahan (jika berkaitan). |
| Nilai Selepas (After Value) | Nilai data selepas perubahan (jika berkaitan). |
| Keputusan (Outcome) | Status: Berjaya (Success) atau Gagal (Failure). |

#### 3.6.3 Ciri Keselamatan Audit

* Rekod audit bersifat **tambah sahaja** (Append-Only) — tiada pengguna, termasuk Pentadbir Sistem, boleh mengubah suai atau memadam entri audit.
* Sokongan penjanaan laporan audit mengikut tempoh, pengguna, jenis tindakan, dan modul.
* Pengekalan rekod audit minimum tiga puluh enam (36) bulan atau mengikut polisi pengekalan data organisasi.

---

### 3.7 Modul Pemberitahuan (Notification Module)

**Tujuan:** Memastikan pihak berkepentingan menerima makluman tepat pada masanya berhubung status KPI, tarikh akhir pelaporan, dan isu data.

#### 3.7.1 Saluran Pemberitahuan

| Saluran | Keterangan |
|---|---|
| **Emel** (Email Notification) | Pemberitahuan dihantar ke alamat emel berdaftar pengguna melalui protokol SMTP yang disulitkan (TLS/SSL). |
| **Pemberitahuan Dalam Aplikasi** (In-App Push Notification) | Pemberitahuan masa nyata yang dipaparkan dalam antara muka sistem semasa pengguna aktif. |

#### 3.7.2 Peristiwa Pencetus Pemberitahuan (Notification Triggers)

* **Tarikh Akhir KPI:** Peringatan automatik pada 14 hari, 7 hari, dan 1 hari sebelum tarikh akhir kemasukan data KPI.
* **Status Muat Naik Data:** Pemberitahuan kejayaan atau kegagalan muat naik fail Excel, termasuk ringkasan ralat.
* **Kelulusan Data:** Pemberitahuan kepada Pengendali Data apabila data diluluskan, ditolak, atau memerlukan pembetulan.
* **Skor Risiko Tinggi:** Amaran automatik apabila KPI mencapai skor risiko melebihi 60 (Kritikal).
* **Perubahan Peranan:** Pemberitahuan kepada pengguna apabila peranan atau kebenaran mereka dikemaskini.

#### 3.7.3 Keutamaan Pemberitahuan

* **Kritikal** (Critical): Kegagalan muat naik, KPI skor risiko merah — dihantar segera melalui emel dan dalam aplikasi.
* **Penting** (Important): Tarikh akhir menjelang, kelulusan tertangguh — dihantar melalui emel dan dalam aplikasi.
* **Maklumat** (Informational): Pengesahan tindakan berjaya — dalam aplikasi sahaja.

---

### 3.8 Modul Integrasi (Integration Module)

**Tujuan:** Menyediakan antara muka pengaturcaraan aplikasi (Application Programming Interface, API) yang membolehkan pertukaran data dengan sistem luaran secara selamat dan piawai.

#### 3.8.1 Rekabentuk API

* **Piawaian:** API RESTful (Representational State Transfer) dengan format pertukaran data JSON (JavaScript Object Notation).
* **Pengesahan API:** Pengesahan berasaskan token (Token-Based Authentication) menggunakan Laravel Sanctum dengan masa tamat token (Token Expiry) yang boleh dikonfigurasi.
* **Kawalan Kadar** (Rate Limiting): Had permintaan API ditetapkan bagi mengelakkan penyalahgunaan: 60 permintaan seminit bagi pengguna biasa, 120 permintaan seminit bagi akaun perkhidmatan (Service Account).
* **Versi API** (API Versioning): Sokongan versi API (contoh: `/api/v1/`, `/api/v2/`) bagi memastikan keserasian ke belakang (Backward Compatibility).

#### 3.8.2 Fungsi API Utama

| Endpoint | Kaedah | Fungsi |
|---|---|---|
| `/api/v1/kpi` | GET | Mendapatkan senarai KPI mengikut penapis (jabatan, tahun, status). |
| `/api/v1/kpi/{id}/data` | GET | Mendapatkan data prestasi bagi KPI tertentu. |
| `/api/v1/upload` | POST | Muat naik fail Excel untuk pemprosesan data. |
| `/api/v1/export` | GET | Mengeksport data dalam format JSON atau CSV. |
| `/api/v1/audit-log` | GET | Mendapatkan rekod jejak audit mengikut penapis. |

#### 3.8.3 Format Data Disokong

* **Import:** Microsoft Excel (.xlsx, .xls), CSV (Comma-Separated Values).
* **Export:** JSON, CSV, Microsoft Excel (.xlsx), PDF (untuk laporan).
* Semua pertukaran data API menggunakan penyulitan HTTPS (TLS 1.2 atau lebih tinggi).

---

### 3.9 Modul Dokumentasi (Documentation Module)

**Tujuan:** Menyediakan repositori dokumen digital bersepadu bagi menguruskan semua dokumen rasmi projek, templat, dan bahan rujukan dalam satu lokasi terpusat.

#### 3.9.1 Repositori Dokumen Rasmi

Sistem menyediakan ruang storan digital yang terkawal untuk dokumen berikut:

| Kategori | Dokumen |
|---|---|
| **Dokumen Pembangunan** | Spesifikasi Keperluan Perisian (SRS), Spesifikasi Rekabentuk Perisian (SDS). |
| **Dokumen Ujian** | Kes Ujian Penerimaan Pengguna (UAT), Ujian Penerimaan Prestasi (PAT), Laporan Ujian. |
| **Dokumen Operasi** | Manual Pengguna (User Manual), Manual Pentadbir (Administrator Manual), Prosedur Operasi Standard (SOP). |
| **Dokumen Migrasi** | Laporan Migrasi Data, Pemetaan Data Sumber-ke-Sasaran. |
| **Templat** | Templat Excel piawai bagi setiap jenis KPI, Templat laporan. |

#### 3.9.2 Fungsi Pengurusan Dokumen

* Muat naik dan muat turun dokumen dengan kawalan versi (Document Versioning).
* Kawalan akses berasaskan peranan — dokumen tertentu hanya boleh diakses oleh peranan yang dibenarkan.
* Fungsi carian teks penuh (Full-Text Search) merentas semua dokumen yang dimuat naik.
* Pencatatan jejak audit bagi setiap tindakan muat naik, muat turun, dan kemaskini dokumen.

---

## 4.0 SENI BINA TEKNIKAL (TECHNICAL ARCHITECTURE)

### 4.1 Gambaran Keseluruhan Seni Bina

Sistem dibina berdasarkan **Seni Bina Tiga Lapisan** (Three-Tier Architecture) dengan pendekatan **"API First"** — iaitu setiap fungsi perniagaan teras didedahkan melalui API dalaman sebelum digunakan oleh lapisan persembahan. Pendekatan ini memastikan kebolehskalaan (Scalability), kebolehselenggaraan (Maintainability), dan kebolehintegrasian (Interoperability) jangka panjang.

### 4.2 Tindanan Teknologi (Technology Stack)

| Lapisan | Teknologi | Justifikasi |
|---|---|---|
| **Lapisan Persembahan** (Presentation Layer) | FilamentPHP 3.x | Rangka kerja panel pentadbiran yang matang, menyediakan komponen papan pemuka, borang, jadual, dan widget secara sedia ada. Mengurangkan masa pembangunan antara muka secara signifikan. |
| **Lapisan Aplikasi** (Application Layer) | Laravel 12 | Rangka kerja PHP yang paling meluas digunakan, menyediakan ekosistem lengkap: ORM (Eloquent), baris gilir kerja (Queue), penghantar emel (Mail), dan pengesahan (Validation). |
| **Lapisan Data** (Data Layer) | MySQL 8.x | Pangkalan data relasi yang terbukti stabil, menyokong transaksi ACID, dan sesuai untuk data berstruktur yang memerlukan integriti rujukan. |
| **Cache dan Baris Gilir** (Cache & Queue) | Redis | Penyimpanan dalam ingatan (In-Memory Store) untuk cache sesi (Session Cache), cache pertanyaan (Query Cache), dan pemprosesan baris gilir kerja tak segerak (Asynchronous Job Queue) bagi muat naik fail Excel. |

### 4.3 Lapisan Seni Bina (Architecture Layers)

#### 4.3.1 Lapisan Persembahan (Presentation Layer)

* **Komponen Utama:** FilamentPHP Resources, Pages, Widgets, dan Custom Livewire Components.
* **Fungsi:** Memaparkan papan pemuka analitik, borang kemasukan data, antara muka pengurusan KPI, dan laporan audit.
* **Prinsip:** Lapisan ini tidak mengandungi logik perniagaan — semua pemprosesan data dilakukan melalui panggilan ke Lapisan Aplikasi.

#### 4.3.2 Lapisan Aplikasi (Application Layer)

* **Komponen Utama:** Laravel Controllers, Service Classes, Form Request Validators, Job Queue Workers, dan Event Listeners.
* **Fungsi:**
  * Pengurusan logik perniagaan: pengesahan data, sanitasi input, transformasi data, dan aliran kerja kelulusan.
  * Pemprosesan muat naik Excel secara tak segerak melalui baris gilir kerja Redis.
  * Pengiraan analitik: skor risiko, unjuran KPI, dan pengesanan anomali.
  * Penjanaan pemberitahuan berdasarkan peristiwa sistem (Event-Driven Notifications).
* **Pendekatan API First:** Semua fungsi perniagaan didedahkan sebagai API dalaman (Internal API) yang kemudiannya digunakan oleh Lapisan Persembahan. Ini memastikan antara muka API luaran (External API) sentiasa konsisten dengan logik perniagaan dalaman.

#### 4.3.3 Lapisan Data (Data Layer)

* **Komponen Utama:** MySQL Database, Eloquent ORM Models, Database Migrations, dan Seeders.
* **Struktur Data Utama:**
  * **Jadual Penampan** (Staging Tables): Menyimpan data mentah daripada muat naik Excel sebelum pengesahan.
  * **Jadual Produksi** (Production Tables): Menyimpan data sah yang telah diluluskan — menjadi sumber tunggal kebenaran (Single Source of Truth).
  * **Jadual Audit** (Audit Tables): Menyimpan jejak audit tidak boleh ubah (Immutable Audit Log).
  * **Jadual Rujukan** (Reference Tables): Menyimpan data rujukan statik: senarai jabatan, kod KPI, definisi peranan.
  * **Jadual Metadata** (Metadata Tables): Menyimpan maklumat sumber fail, versi data, dan cap masa operasi.

### 4.4 Aliran Data Keseluruhan (End-to-End Data Flow)

Aliran data keseluruhan sistem digambarkan secara ringkas seperti berikut:

```
Muat Naik Excel ──▶ Jadual Penampan (Status: DRAFT)
       │
       ▼
Pengesahan Struktur ──▶ [Lulus] ──▶ Pengesahan Format & Logik
       │                                      │
  [Gagal]                                [Gagal]
       │                                      │
       ▼                                      ▼
  Status: STRUCTURE_ERROR              Status: VALIDATION_ERROR
       │                                      │
       └──────── Pembetulan Pengguna ─────────┘
                         │
                         ▼
              Status: PENDING_APPROVAL
                         │
                         ▼
              Semakan & Kelulusan Pengurus KPI
                    │              │
               [Lulus]         [Tolak]
                    │              │
                    ▼              ▼
         Jadual Produksi    Status: REJECTED
        (Status: APPROVED)
                    │
                    ▼
          Papan Pemuka Analitik
          (Dashboard & Reporting)
```

---

## 5.0 METODOLOGI PEMBANGUNAN

### 5.1 Pendekatan Metodologi

Pembangunan sistem dilaksanakan menggunakan **Metodologi Agile — Kitaran Hayat Pembangunan Perisian** (Agile Software Development Life Cycle, SDLC) dengan pelaksanaan secara iteratif dan inkremental. Setiap sprint berdurasi dua (2) minggu dengan serahan (Deliverable) yang boleh diukur.

### 5.2 Fasa Pembangunan

| Fasa | Aktiviti Utama | Serahan (Deliverable) |
|---|---|---|
| **Fasa 1: Analisis Keperluan** | Pengumpulan keperluan fungsian dan bukan fungsian, analisis pihak berkepentingan (Stakeholder Analysis), dan definisi skop akhir. | Dokumen SRS (Versi Diluluskan) |
| **Fasa 2: Rekabentuk Sistem** | Rekabentuk seni bina teknikal, skema pangkalan data, aliran data, antara muka pengguna (Wireframes), dan rekabentuk API. | Dokumen SDS, Gambarajah ER, Wireframes |
| **Fasa 3: Pembangunan Iteratif** | Pembangunan modul secara berperingkat mengikut keutamaan, ujian unit (Unit Testing), dan integrasi berterusan (Continuous Integration). | Prototaip berfungsi bagi setiap sprint |
| **Fasa 4: Ujian Sistem** | Ujian integrasi (Integration Testing), ujian prestasi (Performance Testing), ujian keselamatan (Security Testing), dan Ujian Penerimaan Pengguna (UAT). | Laporan UAT, Laporan PAT, Laporan Keselamatan |
| **Fasa 5: Migrasi Data** | Pemindahan dan normalisasi data legasi daripada fail Excel sedia ada ke pangkalan data produksi baharu. | Laporan Migrasi Data, Pemetaan Data |
| **Fasa 6: Pelaksanaan Rasmi (Go-Live)** | Penempatan sistem (Deployment), latihan pengguna, pemantauan pasca pelancaran (Post-Launch Monitoring), dan serah terima. | Manual Pengguna, Manual Pentadbir, Sijil Serah Terima |

### 5.3 Dokumentasi Wajib (Pematuhan KRISA & PPrISA)

Serahan dokumentasi yang wajib disediakan sepanjang pembangunan projek:

| No. | Dokumen | Keterangan |
|---|---|---|
| 1 | **SRS** (Software Requirement Specification) | Spesifikasi keperluan perisian yang lengkap dan diluluskan. |
| 2 | **SDS** (Software Design Specification) | Spesifikasi rekabentuk teknikal termasuk seni bina, skema data, dan API. |
| 3 | **UAT** (User Acceptance Test) | Kes ujian dan laporan penerimaan pengguna. |
| 4 | **PAT** (Performance Acceptance Test) | Laporan ujian prestasi dan penerimaan beban (Load Testing). |
| 5 | **Manual Pengguna** (User Manual) | Panduan penggunaan sistem untuk pengguna akhir. |
| 6 | **Manual Pentadbir** (Administrator Manual) | Panduan pentadbiran dan konfigurasi sistem. |
| 7 | **Laporan Migrasi Data** (Data Migration Report) | Dokumentasi proses migrasi data legasi termasuk pemetaan dan pengesahan. |
| 8 | **Laporan Penilaian Keselamatan** (Security Assessment Report) | Hasil ujian keselamatan dan langkah mitigasi yang dilaksanakan. |

---

## 6.0 PENGURUSAN KESELAMATAN DATA (SECURITY)

Aspek keselamatan sistem dipandu oleh prinsip **Kerahsiaan, Integriti, dan Ketersediaan** (Confidentiality, Integrity, Availability — CIA Triad) serta pematuhan terhadap keperluan KRISA, PPrISA, dan NCII bagi sistem maklumat sektor kerajaan.

### 6.1 Kawalan Akses dan Pengesahan (Access Control & Authentication)

* **RBAC Bertingkat:** Kawalan akses berasaskan peranan dengan enam (6) peringkat peranan seperti dinyatakan dalam Seksyen 3.1.1.
* **Pengesahan Dua Faktor (2FA):** Wajib bagi semua peranan Pentadbir Sistem, Pentadbir Jabatan, dan Pengurus KPI.
* **Pengurusan Sesi:** Tamat masa sesi automatik (Session Timeout) selepas tiga puluh (30) minit tidak aktif. Satu sesi aktif sahaja bagi setiap akaun pengguna pada satu-satu masa (Single Active Session).
* **Polisi Kata Laluan:** Minimum 12 aksara, gabungan huruf besar dan kecil, nombor, dan aksara khas. Kata laluan mesti dikemaskini setiap sembilan puluh (90) hari.

### 6.2 Sanitasi Data dan Pencegahan Suntikan (Data Sanitization & Injection Prevention)

Memandangkan sumber data utama adalah fail hamparan elektronik (Excel), sanitasi data merupakan komponen keselamatan kritikal:

* **Pencegahan Suntikan Formula (Formula Injection Prevention):** Setiap sel data yang bermula dengan aksara `=`, `+`, `-`, `@`, `\t`, atau `\r` akan dilucutkan (Stripped) atau diawali dengan aksara petikan tunggal (Single Quote Prefix) sebelum diproses.
* **Pengesahan Jenis MIME (MIME Type Validation):** Fail yang dimuat naik disahkan berdasarkan jenis MIME sebenar dan bukan hanya sambungan fail (.xlsx).
* **Had Saiz Fail (File Size Limit):** Maksimum 10MB bagi setiap fail muat naik untuk mengelakkan serangan penafian perkhidmatan (Denial of Service, DoS).
* **Pengimbasan Kandungan (Content Scanning):** Pengesanan makro tertanam (Embedded Macros) dan kandungan VBA dalam fail Excel — fail dengan makro aktif akan ditolak secara automatik.
* **Parameterisasi Pertanyaan (Parameterized Queries):** Semua interaksi pangkalan data menggunakan pertanyaan berparameter melalui Eloquent ORM bagi mencegah suntikan SQL (SQL Injection).

### 6.3 Penyulitan Data (Data Encryption)

* **Data Dalam Simpanan (Data-at-Rest):** Lajur data sensitif dalam pangkalan data disulitkan menggunakan penyulitan peringkat aplikasi (Application-Level Encryption) melalui mekanisme penyulitan terbina dalam Laravel (AES-256-CBC).
* **Data Dalam Transit (Data-in-Transit):** Semua komunikasi antara klien dan pelayan menggunakan protokol HTTPS dengan sijil TLS 1.2 atau lebih tinggi. Komunikasi dalaman antara perkhidmatan (Inter-Service Communication) turut disulitkan.
* **Pengurusan Kunci (Key Management):** Kunci penyulitan disimpan secara berasingan daripada pangkalan data dan diuruskan melalui pemboleh ubah persekitaran (Environment Variables) yang dilindungi.

### 6.4 Jejak Audit dan Integriti Data (Audit Trail & Data Integrity)

* Semua aspek jejak audit seperti yang dinyatakan secara terperinci dalam Seksyen 3.6 merupakan komponen keselamatan teras sistem.
* Integriti data dijamin melalui mekanisme berikut:
  * **Pengesahan Data Berlapis** (Multi-Layer Validation) di peringkat Jadual Penampan sebelum data dipindahkan ke Jadual Produksi.
  * **Integriti Rujukan** (Referential Integrity) dikuatkuasakan melalui kekangan kunci asing (Foreign Key Constraints) dalam pangkalan data.
  * **Rekod Tidak Boleh Padam** (Soft Delete): Rekod data produksi tidak dipadam secara fizikal — sebaliknya ditandakan sebagai tidak aktif (Soft Delete) berserta cap masa dan identiti pengguna yang melaksanakan tindakan tersebut.

### 6.5 Pematuhan Infrastruktur Maklumat Kritikal Nasional (NCII Compliance)

Sistem ini direka bentuk untuk mematuhi keperluan pematuhan NCII yang berkaitan:

* Klasifikasi data mengikut tahap sensitiviti yang ditetapkan oleh organisasi.
* Kawalan akses yang ketat kepada data terkelas.
* Keupayaan penjanaan laporan pematuhan (Compliance Report) untuk tujuan audit keselamatan berkala.
* Pelan pemulihan bencana (Disaster Recovery Plan) termasuk prosedur sandaran data (Data Backup) secara berkala.
* Ujian penembusan keselamatan (Penetration Testing) dilaksanakan sekurang-kurangnya sekali setahun atau selepas setiap kemaskini besar (Major Release).

---

## 7.0 KESIMPULAN

Cadangan teknikal dan spesifikasi keperluan perisian ini membentangkan rangka kerja pembangunan **Sistem Integrasi Data dan Papan Pemuka Prestasi Nasional** yang komprehensif, selamat, dan mematuhi piawaian KRISA, PPrISA, serta NCII.

Sistem ini mentransformasikan amalan pemantauan prestasi daripada proses manual yang berpecah-pecah kepada sebuah ekosistem digital bersepadu yang menyokong prinsip **Tadbir Urus Berasaskan Data** (Data-Driven Governance). Melalui repositori pusat, pengesahan data berlapis, analitik ramalan, dan jejak audit yang tidak boleh diubah suai, sistem ini memastikan bahawa setiap keputusan strategik di peringkat nasional disokong oleh data yang sah, tepat, konsisten, dan boleh diaudit.

Pelaksanaan sistem ini bukan sahaja meningkatkan kecekapan operasi pelaporan, malah memperkukuh ketelusan, akauntabiliti, dan kebolehpercayaan data prestasi nasional — selaras dengan aspirasi kerajaan dalam memperkasakan penyampaian perkhidmatan awam melalui transformasi digital yang berterusan.

---

> **Nota:** Dokumen ini adalah cadangan teknikal peringkat perancangan. Butiran pelaksanaan tertakluk kepada kelulusan Jawatankuasa Pemandu Projek dan mungkin disemak semula berdasarkan maklum balas pihak berkepentingan.
