# CADANGAN TEKNIKAL & SPESIFIKASI SISTEM: SISTEM INTEGRASI DATA DAN PAPAN PEMUKA PRESTASI

**Status Dokumen:** Draf Perancangan Awal (Untuk Semakan Teknikal)  
**Klasifikasi:** Terbuka (Sehingga data sebenar dimasukkan)  
**Pematuhan:** KRISA & PPrISA (Sektor Kerajaan Malaysia)

---

## 1.0 PENGENALAN & LATAR BELAKANG

Dokumen ini menyediakan cadangan teknikal dan spesifikasi sistem bagi pembangunan platform integrasi data berasaskan fail hamparan elektronik (Excel) untuk menghasilkan papan pemuka prestasi nasional. Sistem ini menyokong konsep **National Integrated Monitor**, iaitu repositori pusat yang menyatukan data prestasi daripada pelbagai jabatan, agensi, dan program strategik.

Sistem dicadangkan untuk menggantikan proses manual legasi yang tidak seragam (contohnya pengumpulan fail Excel secara emel), seterusnya memperkukuh integriti data, kelulusan tadbir urus, dan ketelusan pelaporan. Melalui automasi pengesahan (validation), normalisasi data, dan analitik papan pemuka, keputusan strategik dapat disokong secara konsisten, tepat dan boleh diaudit.

---

## 2.0 OBJEKTIF PROJEK

Objektif utama projek ini adalah:

1. Menyediakan repositori data terpusat (centralized repository) untuk semua rekod prestasi yang berasal daripada pelbagai sumber Excel.
2. Mengautomasi pengesahan data dan sanitasi input bagi menjamin integriti serta pematuhan keselamatan.
3. Menyokong pemantauan prestasi masa nyata (real-time monitoring) melalui papan pemuka analitik.
4. Memudahkan pengurusan KPI dan inisiatif strategik secara berstruktur, berjadual dan boleh diaudit.
5. Menyediakan asas analitik ramalan (predictive analytics) untuk menyokong penilaian risiko dan tindakan pembetulan.
6. Mewujudkan jejak audit (audit trail) lengkap bagi setiap transaksi data untuk pematuhan KRISA & PPrISA.

---

## 3.0 SKOP PEMBANGUNAN SISTEM

Skop pembangunan merangkumi sembilan (9) modul utama berikut:

### 3.1 Modul Pengurusan Pengguna & Akses

* Pelaksanaan kawalan akses berasaskan peranan (Role-Based Access Control, RBAC).
* Pengurusan profil pengguna, peranan, dan matriks kebenaran.
* Log aktiviti pengguna untuk semua tindakan kritikal (contoh: muat naik, kelulusan, eksport data).

### 3.2 Modul Pengurusan Strategi & KPI

* Pendaftaran inisiatif strategik, KPI, sasaran tahunan dan garis masa pelaksanaan.
* Pemetaan KPI kepada jabatan, program, atau projek.
* Sokongan versi KPI (versioning) bagi perubahan sasaran atau definisi.

### 3.3 Modul Kemasukan Data

* Sokongan input manual dan muat naik pukal (bulk upload) melalui Excel.
* Proses kemasukan data berasaskan **Staging Table → Validation → Production Table** seperti berikut:
 	* Fail Excel dimuat naik ke zon penampan (staging).
 	* Data melalui pengesahan struktur (header, konsistensi lajur) dan format (tarikh/nombor).
 	* Rekod yang sah dipindahkan ke jadual produksi (production table).
 	* Rekod tidak sah direkod sebagai ralat dan dipaparkan untuk pembetulan.
* Sanitasi data bagi mengelakkan serangan formula atau input berbahaya.

### 3.4 Modul Analitik Data & Dashboard

* Paparan visual analitik prestasi dan perbandingan (benchmarking).
* Pemantauan prestasi mengikut KPI, jabatan, serta garis masa.
* Penunjuk prestasi utama (KPI status) secara dinamik dan konsisten.

### 3.5 Modul AI & Analitik Ramalan

* **KPI Forecasting:** Unjuran prestasi KPI menggunakan model statistik (ARIMA) atau rangkaian neural (Neural Network).
* **Risk Scoring:** Penjanaan skor risiko automatik bagi KPI yang berpotensi tidak mencapai sasaran.
* **Anomaly Detection:** Pengesanan corak luar biasa atau data tidak konsisten semasa muat naik Excel.
* Mekanisme AI ini bertujuan menyokong keputusan awal dan cadangan tindakan pembetulan.

### 3.6 Modul Pemantauan Audit

* Jejak audit penuh (audit trail) bagi semua transaksi data.
* Rekod aktiviti merangkumi pengguna, masa, jenis tindakan dan kesan perubahan.
* Sokongan laporan audit untuk tujuan pematuhan dan penyiasatan.

### 3.7 Modul Pemberitahuan

* Notifikasi emel dan push notification untuk:
 	* Tarikh akhir KPI.
 	* Kegagalan data atau ralat muat naik.
 	* Perubahan status KPI atau kelulusan.

### 3.8 Modul Integrasi

* API import/export bagi membolehkan integrasi dengan sistem luaran.
* Sokongan format CSV dan Excel untuk pertukaran data.
* Piawaian integrasi memastikan konsistensi data antara sistem.

### 3.9 Modul Dokumentasi

* Penyediaan dokumen rasmi termasuk:
 	* SRS (Software Requirement Specification).
 	* SDS (Software Design Specification).
 	* UAT (User Acceptance Test) dan PAT.
 	* Manual Pengguna (User Manual) dan Manual Pentadbir.

---

## 4.0 SENI BINA TEKNIKAL (TECHNICAL ARCHITECTURE)

Seni bina dicadangkan berasaskan model ETL berjadual (Opsyen B) dengan tiga lapisan utama:

### 4.1 Presentation Layer (Lapisan Persembahan)

* Antara muka pengguna dan papan pemuka dibina menggunakan FilamentPHP.
* Paparan laporan, KPI, dan status prestasi dipersembahkan secara dinamik.

### 4.2 Application Layer (Lapisan Aplikasi)

* Laravel 12 sebagai rangka kerja teras aplikasi.
* Pengurusan logik perniagaan termasuk pengesahan, sanitasi, dan transformasi data.
* API integrasi untuk import/export data bagi sistem luaran.

### 4.3 Data Layer (Lapisan Data)

* MySQL sebagai pangkalan data relasi.
* Struktur data mengekalkan rekod asal (staging) dan data sah (production).
* Pencatatan metadata (contoh: sumber fail, masa muat naik, pengguna).

---

## 5.0 METODOLOGI PEMBANGUNAN

Metodologi pembangunan adalah **Agile Software Development Life Cycle (SDLC)** dengan fasa berikut:

1. **Analisis Keperluan** — Pengumpulan keperluan dan definisi skop fungsi.
2. **Rekabentuk Sistem** — Rekabentuk seni bina, modul, dan aliran data.
3. **Pembangunan (Laravel)** — Pembangunan iteratif bagi modul dan integrasi.
4. **Ujian (UAT/PAT)** — Pengesahan fungsian dan penerimaan pengguna.
5. **Migrasi Data** — Pemindahan dan normalisasi data sedia ada.
6. **Go-Live** — Pelaksanaan rasmi dan pemantauan awal.

**Dokumentasi Wajib (KRISA & PPrISA):**

* SRS (Software Requirement Specification).
* SDS (Software Design Specification).
* UAT dan PAT.
* Manual Pengguna dan Manual Pentadbir.

---

## 6.0 ASPEK KESELAMATAN & PEMATUHAN (SECURITY)

Aspek keselamatan dipandu oleh prinsip **Kerahsiaan, Integriti, dan Ketersediaan (CIA)** serta pematuhan NCII.

1. **Kawalan Akses (RBAC):** Akses pengguna dikawal berdasarkan peranan dan kebenaran.
2. **Sanitasi Data:** Semua input Excel disanitasi untuk mencegah formula injection dan input berbahaya.
3. **Audit Trail:** Setiap tindakan direkod dengan cap masa dan identiti pengguna bagi tujuan pematuhan.
4. **Enkripsi Data (Encryption):** Data sensitif disimpan dan dipindahkan menggunakan mekanisme enkripsi yang selamat.
5. **Pengesanan Anomali:** Pengesanan corak luar biasa untuk menandakan potensi isu keselamatan atau data tidak sah.

---

## 7.0 KESIMPULAN

Cadangan ini menekankan pembangunan sistem integrasi data yang mematuhi KRISA & PPrISA, dengan fokus kepada integriti data, automasi proses, dan sokongan keputusan strategik. Melalui repositori pusat, pengesahan data berlapis, serta analitik ramalan, sistem ini dapat meningkatkan ketelusan pelaporan dan memperkukuh keupayaan pemantauan prestasi nasional.
