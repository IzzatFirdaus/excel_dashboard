# DOKUMEN SPESIFIKASI KEPERLUAN BISNES (BRS)

## SISTEM PEMANTAUAN PRESTASI PENDIDIKAN TINGGI

| | |  
|---|---|  
| **NAMA AGENSI** | BAHAGIAN PENGURUSAN MAKLUMAT |
| **NAMA AGENSI INDUK** | KEMENTERIAN PENDIDIKAN TINGGI |
| **TARIKH DOKUMEN** | 22 MEI 2025 |
| **VERSI DOKUMEN** | 1.0 |

---

## i. Keterangan Dokumen

Dokumen ini menerangkan keperluan bisnes dan pengguna bagi pembangunan Sistem Pemantauan Prestasi Pendidikan Tinggi. Kandungannya merangkumi maklumat terperinci skop bisnes, gambaran keseluruhan sistem, pemegang taruh yang terlibat, keperluan pengurusan bisnes, keperluan pengoperasian bisnes dan keperluan proses bisnes. Dokumen ini akan menjadi input kepada penyediaan Spesifikasi Keperluan Sistem yang akan dibangunkan.

---

## ii. Semakan dan Pengesahan Dokumen

### SEMAKAN DOKUMEN

Dokumen ini disemak oleh pasukan kajian dan analisis sistem.

| Disemak Oleh | Jawatan | Tandatangan | Tarikh |  
|---|---|---|---|  
| Hani Masdiana binti Arshad | Ketua Penolong Setiausaha | | 17 Jun 2025 |

### PENGESAHAN DOKUMEN

Dokumen ini disahkan oleh pemilik bisnes dan sistem yang akan dibangunkan.

| Disahkan Oleh | Jawatan | Tandatangan | Tarikh |  
|---|---|---|---|  
| | | | |

---

## iii. Kawalan Dokumen

| No. Versi | Tarikh | Ringkasan Pindaan | Penyedia |  
|---|---|---|---|  
| 1.0 | 22 Mei 2025 | Dokumen versi pertama sedang disediakan | i) Nur Aishah binti Mohd Noh ii) Siti Norsyuhada binti Zainudin iii) Sahruddin bin Sahari |

---

## iv. Kandungan

| Kandungan | Muka Surat |  
|---|---|  
| KETERANGAN DOKUMEN | i |  
| SEMAKAN DAN PENGESAHAN DOKUMEN | ii |  
| KAWALAN DOKUMEN | iii |  
| KANDUNGAN | iv |  
| SENARAI GAMBARAJAH | vi |  
| SENARAI JADUAL | vii |  
| AKRONIM | viii |  
| SUMBER RUJUKAN | ix |  
| 1. PENGENALAN | 1 |  
| &nbsp;&nbsp;1.1 Tujuan Bisnes | 1 |
| &nbsp;&nbsp;1.2 Skop Bisnes | 1 |
| &nbsp;&nbsp;1.3 Gambaran Keseluruhan Bisnes | 1 |
| &nbsp;&nbsp;1.4 Senarai Pemegang Taruh | 2 |
| 2. KEPERLUAN PENGURUSAN BISNES | 3 |
| &nbsp;&nbsp;2.1 Matlamat dan Objektif | 3 |
| &nbsp;&nbsp;2.2 Arkitektur Bisnes | 3 |
| &nbsp;&nbsp;2.3 Arkitektur Maklumat | 4 |
| 3. KEPERLUAN PENGOPERASIAN BISNES | 5 |
| &nbsp;&nbsp;3.1 KEPERLUAN FUNGSI BISNES | 5 |
| &nbsp;&nbsp;&nbsp;&nbsp;3.1.1 Penggunaan Notasi | 5 |
| &nbsp;&nbsp;&nbsp;&nbsp;3.1.2 Model Fungsi Bisnes | 6 |
| &nbsp;&nbsp;&nbsp;&nbsp;3.1.3 Senarai Pengguna | 9 |
| &nbsp;&nbsp;3.2 KEPERLUAN PROSES BISNES | 10 |
| &nbsp;&nbsp;&nbsp;&nbsp;3.2.1 Penggunaan Notasi | 10 |
| &nbsp;&nbsp;&nbsp;&nbsp;3.2.2 Model dan Definisi Proses Bisnes | 12 |
| 4. PENGIRAAN SAIZ APLIKASI | 45 |
| LAMPIRAN | 46 |

---

## v. Senarai Gambarajah

| No. | Rajah | Muka Surat |  
|---|---|---|  
| Rajah 1 | Gambaran Bisnes Unit HEAD | 2 |  
| Rajah 2 | Arkitektur Bisnes KPT | 4 |  
| Rajah 3 | Arkitektur Maklumat Sistem | 5 |  
| Rajah 4 | Hierarki Fungsi Bisnes Pemantauan Prestasi Pendidikan Tinggi | 7 |  
| Rajah 5 | Aliran Proses PFD-PP-MP-HTP Daftar Maklumat Hala Tuju - Program | 12 |  
| Rajah 6 | Aliran Proses PFD-PP-MP-HTK Daftar Maklumat Hala Tuju - Keberhasilan | 17 |  
| Rajah 7 | Aliran Proses PFD-PP-MP-NRC Daftar Maklumat NRC | 19 |  
| Rajah 8 | Aliran Proses PFD-PP-MP-PM Daftar Maklumat PPPM(PT) | 23 |  
| Rajah 9 | Aliran Proses PFD-PP-HT-PR Daftar Program dan Inisiatif â€“ Hala Tuju | 28 |  
| Rajah 10 | Aliran Proses PFD-PP-HT-KPU Kemas kini Pencapaian dan Ulasan Program - Hala Tuju | 32 |
| Rajah 11 | Aliran Proses PFD-PP-HT-KB Kemas kini Pencapaian Keberhasilan â€“ Hala Tuju | 36 |
| Rajah 12 | Aliran Proses PFD-PP-NRC-PSI Daftar Pencapaian dan Status Inisiatif NRC | 40 |  
| Rajah 13 | Aliran Proses PFD-PP-PM-DS Daftar Sasaran PPPM(PT) | 43 |  
| Rajah 14 | Aliran Proses PFD-PP-PM-PCI Daftar Pencapaian dan Catatan Inisiatif PPPM(PT) | 47 |  
| Rajah 15 | Aliran Proses PFD-PP-DB Papar Dashboard dan Jana Laporan | 51 |  
| Rajah 16 | Aliran Proses PFD-PP-AD-PG Daftar Pengguna | 53 |  
| Rajah 17 | Aliran Proses PFD-PP-AD-PL Daftar Pelan | 55 |  
| Rajah 18 | Aliran Proses PFD-PP-AD-IT Daftar Item | 57 |

---

## vi. Senarai Jadual

| No. | Jadual | Muka Surat |  
|---|---|---|  
| Jadual 1 | Senarai Pemegang Taruh | 3 |  
| Jadual 2 | Notasi Hierarki Fungsi Bisnes | 5 |  
| Jadual 3 | Keterangan Fungsi Bisnes | 8 |  
| Jadual 4 | Senarai Pengguna | 9 |  
| Jadual 5 | Notasi Aliran Proses Bisnes | 10 |  
| Jadual 6 | Definisi Aktiviti PFD-PP-MP-HTP 01 Daftar Fokus Utama | 13 |  
| Jadual 7 | Definisi Aktiviti PFD-PP-MP-HTP 02 Daftar Landasan | 14 |  
| Jadual 8 | Definisi Aktiviti PFD-PP-MP-HTP 03 Kemas kini Maklumat Hala Tuju Program | 15 |  
| Jadual 9 | Definisi Aktiviti PFD-PP-MP-HTK 01 Daftar Maklumat Pelaporan Keberhasilan Mengikut Agensi | 17 |  
| Jadual 10 | Definisi Aktiviti PFD-PP-MP-HTK 02 Kemas kini Maklumat Pelaporan Keberhasilan | 18 |  
| Jadual 11 | Definisi Aktiviti PFD-PP-MP-NRC 01 Daftar Teras | 19 |  
| Jadual 12 | Definisi Aktiviti PFD-PP-MP-NRC 02 Daftar Kategori | 20 |  
| Jadual 13 | Definisi Aktiviti PFD-PP-MP-NRC 03 Daftar Maklumat Inisiatif | 21 |  
| Jadual 14 | Definisi Aktiviti PFD-PP-MP-NRC 04 Kemas kini Maklumat NRC | 22 |  
| Jadual 15 | Definisi Aktiviti PFD-PP-MP-PM 01 Daftar Lonjakan | 23 |  
| Jadual 16 | Definisi Aktiviti PFD-PP-MP-PM 02 Daftar Strategi | 24 |  
| Jadual 17 | Definisi Aktiviti PFD-PP-MP-PM 03 Daftar Inisiatif | 25 |  
| Jadual 18 | Definisi Aktiviti PFD-PP-MP-PM 04 Daftar Program | 26 |  
| Jadual 19 | Definisi Aktiviti PFD-PP-MP-PM 05 Kemas kini Maklumat PPPM(PT) | 28 |  
| Jadual 20 | Definisi Aktiviti PFD-PP-HT-PR 01 Daftar Program & Inisiatif â€“ Hala Tuju | 29 |  
| Jadual 21 | Definisi Aktiviti PFD-PP-HT-PR 02 Kemas kini maklumat Program & Inisiatif | 31 |  
| Jadual 22 | Definisi Aktiviti PFD-PP-HT-PR 03 Pengesahan Ketua Jabatan | 32 |  
| Jadual 23 | Definisi Aktiviti PFD-PP-HT-KPU 01 Pengisian Pencapaian dan Ulasan | 33 |  
| Jadual 24 | Definisi Aktiviti PFD-PP-HT-KPU 02 Pengesahan Ketua Jabatan | 34 |  
| Jadual 25 | Definisi Aktiviti PFD-PP-HT-KPU 03 Verifikasi Data | 35 |  
| Jadual 26 | Definisi Aktiviti PFD-PP-HT-KB 01 Pengisian Pencapaian Keberhasilan | 37 |  
| Jadual 27 | Definisi Aktiviti PFD-PP-HT-KB 02 Pengesahan Ketua Jabatan | 38 |  
| Jadual 28 | Definisi Aktiviti PFD-PP-HT-KB 03 Verifikasi Data | 39 |  
| Jadual 29 | Definisi Aktiviti PFD-PP-NRC-PSI 01 Kemas Kini Pencapaian & Status Inisiatif | 40 |  
| Jadual 30 | Definisi Aktiviti PFD-PP-NRC-PSI 02 Pengesahan Ketua Jabatan | 41 |  
| Jadual 31 | Definisi Aktiviti PFD-PP-NRC-PSI 03 Verifikasi Data | 42 |  
| Jadual 32 | Definisi Aktiviti PFD-PP-PM-DS 01 Daftar Sasaran | 44 |  
| Jadual 33 | Definisi Aktiviti PFD-PP-PM-DS 02 Kemas Kini Maklumat Sasaran | 45 |  
| Jadual 34 | Definisi Aktiviti PFD-PP-PM-DS 03 Pengesahan Ketua Jabatan | 46 |  
| Jadual 35 | Definisi Aktiviti PFD-PP-PM-PCI 01 Pengisian Pencapaian | 47 |  
| Jadual 36 | Definisi Aktiviti PFD-PP-PM-PCI 02 Pengesahan Ketua Jabatan | 49 |  
| Jadual 37 | Definisi Aktiviti PFD-PP-PM-PCI 03 Verifikasi Data | 50 |  
| Jadual 38 | Definisi Aktiviti PFD-PP-DB 01 Papar Dashboard | 51 |  
| Jadual 39 | Definisi Aktiviti PFD-PP-DB 02 Jana Laporan | 52 |  
| Jadual 40 | Definisi Aktiviti PFD-PP-AD-PG 01 Daftar Pengguna Baru | 53 |  
| Jadual 41 | Definisi Aktiviti PFD-PP-AD-PG 02 Kemas kini Profil Pengguna | 54 |  
| Jadual 42 | Definisi Aktiviti PFD-PP-AD-PL 01 Daftar Pelan Baru | 55 |  
| Jadual 43 | Definisi Aktiviti PFD-PP-AD-PL 02 Kemas kini Pelan | 56 |  
| Jadual 44 | Definisi Aktiviti PFD-PP-AD-IT 01 Daftar Item Baru | 57 |  
| Jadual 45 | Definisi Aktiviti PFD-PP-AD-IT 02 Kemas kini Item | 58 |  
| Jadual 46 | Pengiraan Saiz Aplikasi Menggunakan Kaedah Function Point | 59 |

---

## vii. Definisi dan Akronim

### a. Akronim

| Akronim | Keterangan |  
|---|---|  
| BRS | Business Requirement Specification / Spesifikasi Keperluan Bisnes |  
| Unit HEAD | Unit Pengurusan Prestasi dan Penyampaian Pendidikan Tinggi |  
| KPT | Kementerian Pendidikan Tinggi |  
| UA | Universiti Awam |  
| BHG | Bahagian |  
| JBTN | Jabatan |  
| DKICT | Dasar Keselamatan ICT |  
| NRC | National Review Committee / Kajian Semula Dasar Pendidikan Tinggi Nasional |  
| PPPM (PT) | Pelan Pembangunan Pendidikan Malaysia 2015-2025 (Pendidikan Tinggi) |  
| SME | Subject Matter Expert / Pakar Rujuk |  
| KPI | Key Performance Indicator / Indikator Prestasi Utama |  
| YB | Yang Berhormat |  
| KP | Ketua Pengarah |

### b. Definisi

| Terma/Istilah | Definisi |  
|---|---|  
| Champion | Pegawai daripada Bahagian/Jabatan/Agensi/UA yang bertanggungjawab untuk mendaftar inisiatif utama dan mengemas kini pencapaian berdasarkan KPI |  
| Urus Setia | Unit HEAD selaku pemilik sistem yang bertanggungjawab melaksanakan verifikasi data serta analisis dan pemantauan inisiatif utama |  
| Verifikasi Data | Proses semakan dan pengesahan data oleh Unit HEAD setelah disahkan oleh Ketua Jabatan |

---

## viii. Sumber Rujukan

Sumber rujukan yang digunakan dalam penyediaan dokumen adalah:

a) Hala Tuju Pendidikan Tinggi  
b) Kajian Semula Dasar Pendidikan Tinggi Nasional (NRC)  
c) Pelan Pembangunan Pendidikan Malaysia 2015-2025 (Pendidikan Tinggi) (PPPM (PT))  
d) Garis Panduan Sistem Pelaporan Prestasi Pendidikan Tinggi  
e) Polisi Keselamatan Siber KPT  
f) Templat Pelan Tindakan PPPM (PT)  
g) Templat Pelaporan Pelan Tindakan Landasan Hala Tuju Pendidikan Tinggi 2024  
h) Templat Data National Review Committee (NRC)

---

## 1. PENGENALAN

### 1.1 Tujuan Bisnes

Unit Pengurusan Prestasi dan Penyampaian Pendidikan Tinggi (HEAD) (pemilik sistem) bertanggungjawab mengumpul, memantau Key Performance Indicator (KPI) dan melaksanakan analisis data bagi memantau inisiatif utama berikut; Hala Tuju Pendidikan Tinggi, Kajian Semula Dasar Pendidikan Tinggi Nasional (NRC) dan Pelan Pembangunan Pendidikan Malaysia 2015-2025 (Pendidikan Tinggi) (PPPM (PT)).

Pada ketika ini, pengumpulan data dilakukan secara manual dan memerlukan masa yang panjang untuk memproses data-data yang diperoleh. Oleh itu, pemilik sistem mencadangkan satu sistem dibangunkan bagi menangani isu-isu semasa dalam pentadbiran dan pengurusan KPI Kementerian Pendidikan Tinggi (KPT). Sistem tersebut perlu memenuhi keperluan berikut:

a) menyelaras pengumpulan data daripada pelbagai set data;  
b) mengurus perubahan data;  
c) pengurusan semakan dan verifikasi data yang lebih efisien; dan  
d) janaan pelaporan secara real-time.

### 1.2 Skop Bisnes

Projek pembangunan ini merangkumi skop bisnes berikut:

a) meliputi semua urusan berkaitan dengan pengisian data oleh pegawai daripada bahagian/jbtn/agensi/ua;  
b) pengesahan maklumat daripada ketua jabatan bhg/jbtn/agensi/ua;  
c) verifikasi data dan analisis data oleh Unit HEAD; dan  
d) pemantauan pelaporan oleh Unit HEAD dan pengurusan atasan.

### 1.3 Gambaran Keseluruhan Bisnes

Unit HEAD mempunyai peranan dan tanggungjawab dalam memastikan keberkesanan sistem pendidikan tinggi melalui pemantauan prestasi, penyampaian dasar, serta penambahbaikan berterusan dalam sektor pendidikan tinggi. Unit ini turut berperanan dalam memantau dan menilai keberkesanan institusi pendidikan tinggi melalui pengukuran KPI. Data prestasi daripada pelbagai institusi termasuk universiti awam, politeknik, kolej komuniti dan institusi swasta dikumpul dan dianalisis. Selain itu, unit ini juga bertanggungjawab mengeluarkan laporan berkala bagi menilai pencapaian serta mengenal pasti cabaran dalam sektor pendidikan tinggi untuk penambahbaikan berterusan.

**Rajah 1 : Gambaran Bisnes Unit HEAD**

```
[Gambar rajah menunjukkan Unit HEAD berperanan dalam memantau Hala Tuju Pendidikan Tinggi,
Kajian Semula Dasar Pendidikan Tinggi Nasional (NRC) dan PPPM(PT) melalui pengumpulan data,
analisis data dan pelaporan kepada Pengurusan Tertinggi]
```

### 1.4 Senarai Pemegang Taruh

**Jadual 1: Senarai Pemegang Taruh**

| Pemegang Taruh | Keterangan |  
|---|---|  
| YB Menteri | Yang Berhormat Menteri bertanggungjawab dalam memantau dan menilai keberkesanan inisiatif utama yang telah dirancang kementerian berjalan lancar. |  
| YB Timbalan Menteri | Yang Berhormat Timbalan Menteri bertanggung jawab memantau dan menilai keberkesanan inisiatif utama yang telah dirancang kementerian berjalan lancar. |  
| Ketua Setiausaha | Bertanggungjawab dalam memantau dan menilai keberkesanan inisiatif utama kementerian berjalan dengan lancar. |  
| Timbalan Ketua Setiausaha | Bertanggungjawab dalam membantu Ketua Setiausaha dalam memantau dan menilai keberkesanan inisiatif utama kementerian berjalan dengan lancar. |  
| KP Pendidikan Tinggi | Bertanggungjawab dalam merancang, menyelaras, memantau, menilai dan melaporkan pencapaian inisiatif yang telah ditetapkan oleh KPT. |  
| KP Pendidikan Politeknik dan Kolej Komuniti | Bertanggungjawab dalam merancang, menyelaras, memantau, menilai dan melaporkan pencapaian inisiatif yang telah ditetapkan oleh KPT. |  
| Naib Canselor | Bertanggungjawab menyelaras, memantau, menilai dan melaporkan pencapaian inisiatif yang ditetapkan oleh KPT. |  
| Timbalan Naib Canselor | Bertanggungjawab dalam membantu menyelaras, memantau, menilai dan melaporkan pencapaian inisiatif yang telah ditetapkan oleh KPT. |  
| Ketua Agensi (MQA/PTPTN/EMGS) | Bertanggungjawab dalam merancang, menyelaras, memantau, menilai dan melaporkan pencapaian inisiatif yang telah ditetapkan oleh KPT. |  
| Setiausaha/Pengarah Bahagian | Bertanggungjawab dalam membantu melaksana, menyelaras, memantau, menilai dan melaporkan pencapaian inisiatif yang telah ditetapkan oleh KPT. |  
| Pengarah Pusat Strategik Universiti Awam | Bertanggungjawab dalam melaksana, menyelaras, memantau, menilai dan melaporkan pencapaian inisiatif yang telah ditetapkan oleh KPT. |  
| Pengarah Politeknik | Bertanggungjawab melaksana, menyelaras, memantau, menilai dan melaporkan pencapaian inisiatif yang telah ditetapkan oleh KPT. |

---

## 2. KEPERLUAN PENGURUSAN BISNES

### 2.1 Matlamat dan Objektif

Sistem yang akan dibangunkan bertujuan membantu pengurusan dan pemantauan Prestasi Pendidikan Tinggi. Objektif utama sistem dibangunkan adalah untuk mencapai matlamat berikut:

a) menyelaras pengumpulan data dengan data set yang berbeza secara efisien;  
b) mengurus perubahan data dengan memastikan integriti data terpelihara;  
c) mempercepatkan tempoh semakan dan verifikasi data bagi melancarkan proses analisis data; dan  
d) menjana laporan pencapaian secara real-time bagi tujuan pemantauan oleh pihak pengurusan tertinggi.

### 2.2 Arkitektur Bisnes

Arkitektur bisnes KPT telah dibangunkan bagi menerangkan perkhidmatan organisasi dan penyelesaian kepada keperluan bisnes bagi menentukan objektif organisasi yang lebih strategik. Ianya merupakan satu rujukan dalam menerangkan pengurusan keperluan (Requirements Management) pembangunan aplikasi yang akan dibangunkan dan hubung kait dengan pelanggan, perkhidmatan agensi, maklumat (data) dan teknologi.

**Rajah 2 : Arkitektur Bisnes KPT**

```  
[Gambar rajah menunjukkan hubung kait antara Pelanggan (KPT, Agensi, UA, Politeknik),  
Perkhidmatan (Pemantauan Prestasi Pendidikan Tinggi), Sistem Aplikasi (Sistem Pemantauan  
Prestasi Pendidikan Tinggi), Data (Hala Tuju, NRC, PPPM(PT)) dan Teknologi (Rangkaian,  
Pelayan, Keselamatan)]  
```

### 2.3 Arkitektur Maklumat

**Rajah 3 : Arkitektur Maklumat Sistem**

```  
[Gambar rajah menunjukkan hubung kait antara Pengguna (Pengurusan Tertinggi, Urus Setia/HEAD,  
Champion, Pegawai Pengesah), Proses Bisnes (Mengurus Maklumat Prestasi, Mengurus Pelan  
Hala Tuju, Mengurus NRC, Mengurus PPPM(PT), Papar Dashboard & Jana Laporan, Pengurusan  
Pentadbiran) dan Maklumat (Data Prestasi, Data Sasaran, Data Pengguna, Data Pelaporan)]  
```

---

## 3\. KEPERLUAN PENGOPERASIAN BISNES

### 3.1 KEPERLUAN FUNGSI BISNES

#### 3.1.1 Penggunaan Notasi

**Jadual 2 : Notasi Hierarki Fungsi Bisnes**

| Elemen | Keterangan |  
|---|---|  
| Fungsi Bisnes | Digunakan bagi mewakili setiap fungsi bisnes. Labelkan ID Fungsi Bisnes dan Nama Fungsi Bisnes di dalam notasi. |  
| Sintaks Nama Fungsi | `\<kata kerja\> \<kata nama\>` Nama fungsi bisnes hendaklah dimulakan dengan kata kerja dan diikuti kata nama. |  
| ID Fungsi Bisnes | BF-PP-XX-YY Digunakan sebagai konvensyen nama bagi setiap fungsi bisnes yang dibangunkan. Contoh Keterangan Kandungan ID: BF : Ringkasan Teknik Fungsi Bisnes PP: Ringkasan Pemantauan Prestasi XX : Ringkasan Sub Fungsi YY : Ringkasan Fungsi Asas |  
| Penghubung antara fungsi mendatar atau menegak | Penghubung antara fungsi dan sub fungsi menggunakan garis lurus mendatar atau menegak. |  
| Keterangan Fungsian Bisnes | `\<pemegang taruh\> \<kata kerja\> \<prestasi/kekerapan\> \<peristiwa\> \<syarat-syarat\>` Pernyataan yang akan menerangkan suatu fungsian bisnes. |

#### 3.1.2 Model Fungsi Bisnes

Fungsi bisnes disediakan berdasarkan maklumat yang diperoleh melalui bengkel yang telah diadakan bersama pemilik proses daripada Unit HEAD; serta berdasarkan dokumen-dokumen berkaitan proses bisnes yang dirujuk. Fungsi utama dan sub fungsi bisnes telah dikenal pasti selaras dengan tujuan utama pembangunan Sistem Pemantauan Pengurusan Prestasi.

**a) Struktur Hierarki Fungsi Bisnes**

**Rajah 4 : Hierarki Fungsi Bisnes Pemantauan Prestasi Pendidikan Tinggi**

```  
BF-PP (Mengurus dan melaksanakan analisis data bagi memantau prestasi Pendidikan Tinggi)  
â”‚  
â”œâ”€â”€ BF-PP-MP (Mengurus Maklumat Prestasi)  
â”‚   â”œâ”€â”€ BF-PP-MP-HTP (Daftar Maklumat Hala Tuju - Program)  
â”‚   â”œâ”€â”€ BF-PP-MP-HTK (Daftar Maklumat Hala Tuju - Keberhasilan)  
â”‚   â”œâ”€â”€ BF-PP-MP-NRC (Daftar Maklumat NRC)  
â”‚   â””â”€â”€ BF-PP-MP-PM (Daftar Maklumat PPPM(PT))  
â”‚  
â”œâ”€â”€ BF-PP-HT (Mengurus Pelan Hala Tuju Pendidikan Tinggi)  
â”‚   â”œâ”€â”€ BF-PP-HT-PR (Daftar Program dan Inisiatif)  
â”‚   â”œâ”€â”€ BF-PP-HT-KPU (Kemas kini Pencapaian & Ulasan Program)  
â”‚   â””â”€â”€ BF-PP-HT-KB (Kemas kini Pencapaian Keberhasilan)  
â”‚  
â”œâ”€â”€ BF-PP-NRC (Mengurus Kajian Semula Dasar Pendidikan Tinggi)  
â”‚   â””â”€â”€ BF-PP-NRC-PSI (Daftar Pencapaian & Status Inisiatif NRC)  
â”‚  
â”œâ”€â”€ BF-PP-PM (Mengurus PPPM(PT))  
â”‚   â”œâ”€â”€ BF-PP-PM-DS (Daftar Sasaran PPPM(PT))  
â”‚   â””â”€â”€ BF-PP-PM-PCI (Daftar Pencapaian & Catatan Inisiatif PPPM(PT))  
â”‚  
â”œâ”€â”€ BF-PP-DB (Papar Dashboard dan Jana Laporan Prestasi Pendidikan Tinggi)  
â”‚  
â””â”€â”€ BF-PP-AD (Pengurusan Pentadbiran)  
    â”œâ”€â”€ BF-PP-AD-PG (Daftar Pengguna)  
    â”œâ”€â”€ BF-PP-AD-PL (Daftar Pelan)  
    â””â”€â”€ BF-PP-AD-IT (Daftar Item)  
```

**b) Keterangan Fungsi Bisnes**

**Jadual 3 : Keterangan Fungsi Bisnes**

| ID Fungsi Bisnes | Nama Fungsi Bisnes | Keterangan Fungsi Bisnes |  
|---|---|---|  
| BF-PP | Mengurus dan melaksanakan analisis data bagi memantau prestasi Pendidikan Tinggi | Unit HEAD berperanan dalam mengurus dan melaksanakan analisis data bagi memantau prestasi Pendidikan Tinggi. Proses yang terlibat merangkumi mengurus pengguna, mengurus pencapaian dan KPI, mengurus maklumat prestasi dan menjana laporan yang berkaitan. |  
| BF-PP-MP | Mengurus Maklumat Prestasi | Unit HEAD/Urus setia berperanan untuk mengurus maklumat asas yang diperlukan bagi setiap pelan utama. |  
| BF-PP-HT | Mengurus Pelan Hala Tuju Pendidikan Tinggi | Pegawai BHG/JBTN/AGENSI/UA berperanan dalam mengurus program dan inisiatif serta pencapaian keberhasilan yang telah ditetapkan dalam Hala Tuju Pendidikan Tinggi. Manakala Unit HEAD/Urus setia berperanan dalam verifikasi data yang diterima. |  
| BF-PP-NRC | Mengurus Kajian Semula Dasar Pendidikan Tinggi | Pegawai BHG/JBTN/AGENSI/UA berperanan dalam mengurus pencapaian dan inisiatif yang telah dipersetujui dalam Dasar Pendidikan Tinggi. Manakala Unit HEAD/Urus setia berperanan dalam verifikasi data yang diterima. |  
| BF-PP-PM | Mengurus PPPM(PT) | Pegawai BHG/JBTN/AGENSI/UA berperanan dalam mengurus pencapaian berdasarkan lonjakan yang terdapat dalam PPPM(PT). Manakala Unit HEAD/Urus setia berperanan dalam verifikasi data yang diterima. |  
| BF-PP-DB | Papar Dashboard dan Jana Laporan Prestasi Pendidikan Tinggi | Unit HEAD/Urus setia berperanan dalam menjana dan memapar maklumat pencapaian prestasi semasa melalui dashboard dan penjanaan laporan. Manakala Pengurusan Tertinggi boleh memantau pelaporan tersebut pada bila-bila masa. |  
| BF-PP-AD | Pengurusan Pentadbiran | Unit HEAD/Urus setia berperanan dalam pengurusan pentadbiran yang merangkumi proses pengurusan pengguna, daftar pelan dan daftar item. |  
| BF-PP-MP-HTP | Daftar Maklumat Hala Tuju - Program | Unit HEAD/Urus setia berperanan untuk mendaftar maklumat asas yang diperlukan bagi Hala Tuju Pendidikan Tinggi (Program) |  
| BF-PP-MP-HTK | Daftar Maklumat Hala Tuju - Keberhasilan | Unit HEAD/Urus setia berperanan untuk mendaftar maklumat asas yang diperlukan bagi Hala Tuju Pendidikan Tinggi (Keberhasilan) |  
| BF-PP-MP-NRC | Daftar Maklumat NRC | Unit HEAD/Urus setia berperanan untuk mendaftar maklumat asas yang diperlukan bagi Dasar Pendidikan Tinggi |  
| BF-PP-MP-PM | Daftar Maklumat PPPM(PT) | Unit HEAD/Urus setia berperanan untuk mendaftar maklumat asas yang diperlukan bagi PPPM(PT). |  
| BF-PP-HT-PR | Daftar Program dan Inisiatif | Pegawai BHG/JBTN/AGENSI/UA berperanan untuk mendaftarkan program dan inisiatif dalam Hala Tuju Pendidikan Tinggi. |  
| BF-PP-HT-KPU | Kemas kini Pencapaian & Ulasan Program | Pegawai BHG/JBTN/AGENSI/UA berperanan dalam mengemas kini pencapaian dan ulasan program telah didaftarkan. |  
| BF-PP-HT-KB | Kemas kini Pencapaian Keberhasilan | Pegawai BHG/JBTN/AGENSI/UA berperanan dalam mengemas kini pencapaian keberhasilan yang telah dirancang dalam Hala Tuju Pendidikan Tinggi. |  
| BF-PP-NRC-PSI | Daftar Pencapaian & Status Inisiatif | Pegawai BHG/JBTN/AGENSI/UA berperanan untuk mendaftar pencapaian dan status inisiatif yang telah dipersetujui dalam Dasar Pendidikan Tinggi. |  
| BF-PP-PM-DS | Daftar Sasaran PPPM(PT) | Pegawai BHG/JBTN/AGENSI/UA berperanan untuk mendaftarkan sasaran berdasarkan lonjakan yang terdapat dalam PPPM(PT). |

#### 3.1.3 Senarai Pengguna

**Jadual 4: Senarai Pengguna**

| Pengguna | Keterangan |  
|---|---|  
| Pengurusan Tertinggi | Pengurusan Tertinggi KPT selaku pemegang taruh Sistem Pemantauan Prestasi Pendidikan Tinggi berperanan untuk memantau prestasi pendidikan tinggi berdasarkan KPI yang telah ditetapkan dan menilai keberkesanan inisiatif utama yang telah dirancang daripada pelbagai peringkat. |  
| Urus setia (Unit HEAD) | Unit HEAD selaku pemilik Sistem Pemantauan Prestasi Pendidikan Tinggi berperanan untuk melaksanakan verifikasi data yang didaftar atau dikemas kini oleh pegawai daripada BHG/JBTN/AGENSI/UA serta melaksanakan analisis dan memantau inisiatif utama yang telah dirancang. |  
| Champion (Pegawai daripada BHG/JBTN/AGENSI/UA) | Pegawai daripada BHG/JBTN/AGENSI/UA bertanggungjawab untuk mendaftar inisiatif utama dan mengemas kini pencapaian berdasarkan KPI yang telah ditetapkan. |  
| Pegawai Pengesah BHG/JBTN/AGENSI/UA | Pegawai pengesah daripada BHG/JBTN/AGENSI/UA berperanan untuk mengesahkan data dan pencapaian yang didaftar atau dikemas kini oleh champion sebelum maklumat tersebut diverifikasi dan dianalisis oleh Unit HEAD. |

### 3.2 KEPERLUAN PROSES BISNES

#### 3.2.1 Penggunaan Notasi

**Jadual 5 : Notasi Aliran Proses Bisnes**

| Elemen | Keterangan |  
|---|---|  
| Activity | Digunakan bagi mewakili setiap aktiviti. Labelkan ID Aktiviti Bisnes dan Nama Aktiviti Bisnes di dalam notasi. |  
| Control Flow/Edge | Digunakan untuk menghubungkan satu elemen notasi kepada notasi-notasi berikutnya. |  
| Swimlane | Digunakan untuk mengumpulkan aktiviti-aktiviti yang di bawah satu-satu peranan. Nama peranan dilabelkan berdasarkan individu, unit bisnes, organisasi atau sistem luaran. |  
| Initial Node | Digunakan untuk menggambarkan permulaan bagi proses. |  
| Activity Final Node | Digunakan untuk menamatkan keseluruhan aliran aktiviti. |  
| Flow Final Node | Digunakan untuk memberhentikan aliran aktiviti yang spesifik sahaja. |  
| Send Signal Action | Digunakan untuk penghantaran isyarat (notifikasi). Nama isyarat yang dihantar perlu dicatatkan di dalam notasi berkenaan. |  
| Accept Event Action | Digunakan untuk penerimaan isyarat (notifikasi). Nama isyarat yang diterima perlu dicatatkan di dalam notasi berkenaan. |  
| Decision | Digunakan untuk memisahkan satu aliran proses kepada beberapa aliran proses berbeza berdasarkan salah satu kriteria keputusan yang ingin dipenuhi. Labelkan kriteria keputusan seperti "Ya" atau "Tidak" bagi setiap cabang aliran proses berkenaan. |  
| Merge | Digunakan untuk menggabungkan semula aliran-aliran proses yang berlainan supaya hanya satu aliran proses sahaja yang disambungkan kepada aktiviti seterusnya. |  
| Fork | Digunakan untuk memisahkan aliran proses kepada beberapa aliran proses berbeza bagi aktiviti-aktiviti yang dilaksanakan secara selari. |  
| Join | Digunakan untuk menggabungkan semula aliran-aliran proses bagi aktiviti-aktiviti yang berjalan secara selari supaya proses dapat disambungkan kepada aktiviti seterusnya. |  
| Note | Digunakan untuk mencatatkan nota ringkas bagi satu-satu aktiviti. Kandungan nota dicatatkan di dalam ruangan notasi tersebut. |  
| ID Fungsi Bisnes | PFD-PP-XX-YY Digunakan sebagai konvensyen nama dan nombor bagi setiap tajuk rajah PFD yang dibangunkan. Keterangan Kandungan ID: PFD : Ringkasan Proses Flow Diagram PP : Ringkasan Pemantauan Prestasi XX : Ringkasan Nama Sub Fungsi YY : Ringkasan Nama Fungsi Asas |  
| ID Aktiviti Bisnes | PFD-PP-XX-YY-99 Digunakan sebagai konvensyen nama dan nombor bagi setiap aktiviti yang terkandung dalam satu-satu PFD. Keterangan Kandungan ID: PFD : Ringkasan Proses Flow Diagram PP : Ringkasan Pemantauan Prestasi XX : Ringkasan Nama Sub Fungsi YY : Ringkasan Nama Fungsi Asas 99 : Nombor Rujukan Aktiviti Bisnes |

#### 3.2.2 Model dan Definisi Proses Bisnes

##### a) PFD-PP-MP-HTP Daftar Maklumat Hala Tuju - Program

**Rajah 5 : Aliran Proses PFD-PP-MP-HTP Daftar Maklumat Hala Tuju - Program**

```  
[Rajah aliran proses menunjukkan Urus setia memulakan proses, mendaftar fokus utama,  
mendaftar landasan, dan membuat kemas kini maklumat hala tuju program]  
```

**Jadual 6 : Definisi Aktiviti PFD-PP-MP-HTP 01 Daftar Fokus Utama**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-HTP |  
| Nama Fungsi | Daftar Maklumat Hala Tuju - Program |  
| Rujukan Aktiviti | PFD-PP-MP-HTP 01 |  
| Nama Aktiviti | Daftar Fokus Utama |  
| Keterangan Aktiviti | Mendaftar fokus utama bagi Pelan Hala Tuju Pendidikan Tinggi. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-MP-HTP 02 Daftar Landasan atau PFD-PP-MP-HTP 03 Kemas kini maklumat Hala Tuju Program |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem dan mendaftar butiran Fokus Utama bagi Pelan Hala Tuju Pendidikan Tinggi. |  
| **Penggunaan Maklumat:** | Maklumat Fokus (C) 1\. Nama Fokus Utama 2\. Butiran Fokus Utama |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 7 : Definisi Aktiviti PFD-PP-MP-HTP 02 Daftar Landasan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-HTP |  
| Nama Fungsi | Daftar Maklumat Hala Tuju - Program |  
| Rujukan Aktiviti | PFD-PP-MP-HTP 02 |  
| Nama Aktiviti | Daftar Landasan |  
| Keterangan Aktiviti | Mendaftar landasan bagi Pelan Hala Tuju Pendidikan Tinggi. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-MP-HTP 01 Daftar Fokus Utama |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-MP-HTP 03 Kemas kini maklumat Hala Tuju Program |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem dan mendaftarkan butiran Landasan bagi Pelan Hala Tuju Pendidikan Tinggi. |  
| **Penggunaan Maklumat:** | Maklumat Landasan (C) 1\. Nama Landasan 2\. Butiran Landasan |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 8 : Definisi Aktiviti PFD-PP-MP-HTP 03 Kemas kini Maklumat Hala Tuju Program**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-HTP |  
| Nama Fungsi | Daftar Maklumat Hala Tuju - Program |  
| Rujukan Aktiviti | PFD-PP-MP-HTP 03 |  
| Nama Aktiviti | Kemas kini Maklumat Hala Tuju Program |  
| Keterangan Aktiviti | Mengemas kini maklumat Hala Tuju Program. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-MP-HTP 01 Daftar Fokus atau PFD-PP-MP-HTP 02 Daftar Landasan |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem untuk mengemas kini maklumat hala tuju yang diperlukan. 2\. Maklumat yang telah digunakan di modul yang lain tidak boleh dipadam atau dikemas kini. |  
| **Penggunaan Maklumat:** | Maklumat Fokus (RUD) 1\. Nama Fokus Utama 2\. Butiran Fokus Utama Maklumat Landasan (RUD) 1\. Nama Landasan 2\. Butiran Landasan |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

##### b) PFD-PP-MP-HTK Daftar Maklumat Hala Tuju - Keberhasilan

**Rajah 6 : Aliran Proses PFD-PP-MP-HTK Daftar Maklumat Hala Tuju - Keberhasilan**

```  
[Rajah aliran proses menunjukkan Urus setia memulakan proses, mendaftar maklumat pelaporan  
keberhasilan, dan membuat kemas kini maklumat pelaporan keberhasilan]  
```

**Jadual 9 : Definisi Aktiviti PFD-PP-MP-HTK 01 Daftar Maklumat Pelaporan Keberhasilan Mengikut Agensi**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-HTK |  
| Nama Fungsi | Daftar Maklumat Hala Tuju - Keberhasilan |  
| Rujukan Aktiviti | PFD-PP-MP-HTK 01 |  
| Nama Aktiviti | Daftar Maklumat Pelaporan Keberhasilan Mengikut Agensi |  
| Keterangan Aktiviti | Mendaftar maklumat pelaporan keberhasilan mengikut agensi. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-MP-HTK 02 Kemas kini maklumat pelaporan keberhasilan |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem untuk mendaftar butiran pelaporan keberhasilan bagi Pelan Hala Tuju Pendidikan Tinggi. |  
| **Penggunaan Maklumat:** | Maklumat Keberhasilan (C) 1\. Nama Sumber 2\. Butiran Sumber 3\. Unit Pengukuran 4\. Frekuensi Pelaporan |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 10 : Definisi Aktiviti PFD-PP-MP-HTK 02 Kemas kini Maklumat Pelaporan Keberhasilan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-HTK |  
| Nama Fungsi | Daftar Maklumat Hala Tuju - Keberhasilan |  
| Rujukan Aktiviti | PFD-PP-MP-HTK 02 |  
| Nama Aktiviti | Kemas kini Maklumat Pelaporan Keberhasilan |  
| Keterangan Aktiviti | Mengemas kini maklumat pelaporan keberhasilan. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-MP-HTK 01 Daftar Maklumat Pelaporan Keberhasilan Mengikut Agensi |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem untuk mengemas kini butiran pelaporan keberhasilan bagi Pelan Hala Tuju Pendidikan Tinggi. 2\. Maklumat yang telah digunakan di modul yang lain tidak boleh dipadam atau dikemas kini. |  
| **Penggunaan Maklumat:** | Maklumat Keberhasilan (RUD) 1\. Nama Sumber 2\. Butiran Sumber 3\. Unit Pengukuran 4\. Frekuensi Pelaporan |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

##### c) PFD-PP-MP-NRC Daftar Maklumat NRC

**Rajah 7 : Aliran Proses PFD-PP-MP-NRC Daftar Maklumat NRC**

```  
[Rajah aliran proses menunjukkan Urus setia memulakan proses, mendaftar teras, mendaftar kategori,  
mendaftar maklumat inisiatif, dan membuat kemas kini maklumat NRC]  
```

**Jadual 11 : Definisi Aktiviti PFD-PP-MP-NRC 01 Daftar Teras**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-NRC |  
| Nama Fungsi | Daftar Maklumat NRC |  
| Rujukan Aktiviti | PFD-PP-MP-NRC 01 |  
| Nama Aktiviti | Daftar Teras |  
| Keterangan Aktiviti | Mendaftar teras bagi maklumat NRC. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-MP-NRC 04 Kemas kini maklumat NRC |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem untuk mendaftar maklumat Teras bagi NRC. |  
| **Penggunaan Maklumat:** | Maklumat Teras (C) 1\. Nama Teras 2\. Butiran Teras |  
| **Polisi dan Dasar Berkaitan** | 1\. Kajian Semula Dasar Pendidikan Tinggi Nasional (NRC) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 12 : Definisi Aktiviti PFD-PP-MP-NRC 02 Daftar Kategori**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-NRC |  
| Nama Fungsi | Daftar Maklumat NRC |  
| Rujukan Aktiviti | PFD-PP-MP-NRC 02 |  
| Nama Aktiviti | Daftar Kategori |  
| Keterangan Aktiviti | Mendaftar kategori bagi maklumat NRC. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-MP-NRC 01 Daftar Teras |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-MP-NRC 04 Kemas kini maklumat NRC |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem untuk mendaftar maklumat Kategori bagi NRC. |  
| **Penggunaan Maklumat:** | Maklumat Kategori (C) 1\. Nama Kategori 2\. Butiran Kategori |  
| **Polisi dan Dasar Berkaitan** | 1\. Kajian Semula Dasar Pendidikan Tinggi Nasional (NRC) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 13 : Definisi Aktiviti PFD-PP-MP-NRC 03 Daftar Maklumat Inisiatif**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-NRC |  
| Nama Fungsi | Daftar Maklumat NRC |  
| Rujukan Aktiviti | PFD-PP-MP-NRC 03 |  
| Nama Aktiviti | Daftar Maklumat Inisiatif |  
| Keterangan Aktiviti | Mendaftar maklumat inisiatif bagi maklumat NRC. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-MP-NRC 01 Daftar Teras dan PFD-PP-MP-NRC 02 Daftar Kategori |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-MP-NRC 04 Kemas kini maklumat NRC |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem untuk mendaftar maklumat Inisiatif bagi NRC. |  
| **Penggunaan Maklumat:** | Maklumat Inisiatif 1\. Nama Teras (R) 2\. Nama Kategori (R) 3\. Nama Inisiatif (C) 4\. KPI (C) 5\. Sasaran (C) 6\. Jabatan/Bahagian/Agensi/UA (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Kajian Semula Dasar Pendidikan Tinggi Nasional (NRC) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 14 : Definisi Aktiviti PFD-PP-MP-NRC 04 Kemas kini Maklumat NRC**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-NRC |  
| Nama Fungsi | Daftar Maklumat NRC |  
| Rujukan Aktiviti | PFD-PP-MP-NRC 04 |  
| Nama Aktiviti | Kemas kini Maklumat NRC |  
| Keterangan Aktiviti | Mengemas kini maklumat NRC. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-MP-NRC 01 Daftar Teras atau PFD-PP-MP-NRC 02 Daftar Kategori atau PFD-PP-MP-NRC 03 Daftar Maklumat Inisiatif |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem untuk mengemas kini maklumat NRC yang diperlukan. 2\. Maklumat yang telah digunakan di modul yang lain tidak boleh dipadam atau dikemas kini. |  
| **Penggunaan Maklumat:** | Maklumat Teras (RUD) 1\. Nama Teras 2\. Butiran Teras Maklumat Kategori (RUD) 1\. Nama Kategori 2\. Butiran Kategori Maklumat Inisiatif (RUD) 1\. Nama Inisiatif 2\. Butiran Inisiatif 3\. KPI 4\. Sasaran 5\. Jabatan/Bahagian/Agensi/UA |  
| **Polisi dan Dasar Berkaitan** | 1\. Kajian Semula Dasar Pendidikan Tinggi Nasional (NRC) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

##### d) PFD-PP-MP-PM Daftar Maklumat PPPM(PT)

**Rajah 8 : Aliran Proses PFD-PP-MP-PM Daftar Maklumat PPPM(PT)**

```  
[Rajah aliran proses menunjukkan Urus setia memulakan proses, mendaftar lonjakan, mendaftar strategi,  
mendaftar inisiatif, mendaftar program, dan membuat kemas kini maklumat PPPM(PT)]  
```

**Jadual 15 : Definisi Aktiviti PFD-PP-MP-PM 01 Daftar Lonjakan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-PM |  
| Nama Fungsi | Daftar Maklumat PPPM(PT) |  
| Rujukan Aktiviti | PFD-PP-MP-PM 01 |  
| Nama Aktiviti | Daftar Lonjakan |  
| Keterangan Aktiviti | Mendaftar lonjakan bagi maklumat PPPM(PT). |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-MP-PM 05 Kemas kini Maklumat PPPM(PT) |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem untuk mendaftarkan maklumat Lonjakan bagi PPPM(PT). |  
| **Penggunaan Maklumat:** | Maklumat Lonjakan (C) 1\. Nama Lonjakan 2\. Butiran Lonjakan |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Pembangunan Pendidikan Malaysia 2015-2025 (Pendidikan Tinggi) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 16 : Definisi Aktiviti PFD-PP-MP-PM 02 Daftar Strategi**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-PM |  
| Nama Fungsi | Daftar Maklumat PPPM (PT) |  
| Rujukan Aktiviti | PFD-PP-MP-PM 02 |  
| Nama Aktiviti | Daftar Strategi |  
| Keterangan Aktiviti | Mendaftar strategi bagi maklumat PPPM(PT). |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-MP-PM 01 Daftar Lonjakan |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-MP-PM 05 Kemas kini Maklumat PPPM(PT) |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem untuk mendaftarkan maklumat Strategi bagi PPPM(PT). |  
| **Penggunaan Maklumat:** | Maklumat Strategi 1\. Lonjakan (R) 2\. Nama Strategi (C) 3\. Butiran Strategi (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Pembangunan Pendidikan Malaysia 2015-2025 (Pendidikan Tinggi) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 17 : Definisi Aktiviti PFD-PP-MP-PM 03 Daftar Inisiatif**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-PM |  
| Nama Fungsi | Daftar Maklumat PPPM(PT) |  
| Rujukan Aktiviti | PFD-PP-MP-PM 03 |  
| Nama Aktiviti | Daftar Inisiatif |  
| Keterangan Aktiviti | Mendaftar inisiatif bagi maklumat PPPM(PT). |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-MP-PM 02 Daftar Strategi |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-MP-PM 05 Kemas kini Maklumat PPPM(PT) |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem untuk mendaftarkan maklumat Inisiatif bagi PPPM(PT). |  
| **Penggunaan Maklumat:** | Maklumat Inisiatif 1\. Lonjakan (R) 2\. Strategi (R) 3\. Nama Inisiatif (C) 4\. Butiran Inisiatif (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Pembangunan Pendidikan Malaysia 2015-2025 (Pendidikan Tinggi) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 18 : Definisi Aktiviti PFD-PP-MP-PM 04 Daftar Program**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-PM |  
| Nama Fungsi | Daftar Maklumat PPPM(PT) |  
| Rujukan Aktiviti | PFD-PP-MP-PM 04 |  
| Nama Aktiviti | Daftar Program |  
| Keterangan Aktiviti | Mendaftar program bagi maklumat PPPM(PT). |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-MP-PM 03 Daftar Inisiatif |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-MP-PM 05 Kemas kini Maklumat PPPM(PT) |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem untuk mendaftarkan maklumat Program bagi PPPM(PT). |  
| **Penggunaan Maklumat:** | Maklumat Program 1\. Lonjakan (R) 2\. Strategi (R) 3\. Inisiatif (R) 4\. Nama Program (C) 5\. Deskripsi Program (C) 6\. KPI (C) 7\. Bahagian/Jabatan/Agensi/UA (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Pembangunan Pendidikan Malaysia 2015-2025 (Pendidikan Tinggi) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 19 : Definisi Aktiviti PFD-PP-MP-PM 05 Kemas kini Maklumat PPPM(PT)**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-MP-PM |  
| Nama Fungsi | Daftar Maklumat PPPM(PT) |  
| Rujukan Aktiviti | PFD-PP-MP-PM 05 |  
| Nama Aktiviti | Kemas kini Maklumat PPPM(PT) |  
| Keterangan Aktiviti | Mengemas kini maklumat PPPM(PT). |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-MP-PM 01 Daftar Lonjakan atau PFD-PP-MP-PM 02 Daftar Strategi atau PFD-PP-MP-PM 03 Daftar Inisiatif atau PFD-PP-MP-PM 04 Daftar Program |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia hendaklah log masuk ke sistem untuk mengemas kini maklumat PPPM(PT) yang diperlukan. 2\. Maklumat yang telah digunakan di modul yang lain tidak boleh dipadam atau dikemas kini. |  
| **Penggunaan Maklumat:** | Maklumat Lonjakan (RUD) 1\. Nama Lonjakan 2\. Butiran Lonjakan Maklumat Strategi 1\. Lonjakan (R) 2\. Nama Strategi (RUD) 3\. Butiran Strategi (RUD) Maklumat Inisiatif 1\. Lonjakan (R) 2\. Strategi (R) 3\. Nama Inisiatif (RUD) 4\. Butiran Inisiatif (RUD) Maklumat Program 1\. Lonjakan (R) 2\. Strategi (R) 3\. Inisiatif (R) 4\. Nama Program (RUD) 5\. Deskripsi Program (RUD) 6\. KPI (RUD) 7\. Bahagian/Jabatan/Agensi/UA (RUD) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Pembangunan Pendidikan Malaysia 2015-2025 (Pendidikan Tinggi) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

##### e) PFD-PP-HT-PR Daftar Program dan Inisiatif - Hala Tuju

**Rajah 9 : Aliran Proses PFD-PP-HT-PR Daftar Program dan Inisiatif â€“ Hala Tuju**

```  
[Rajah aliran proses menunjukkan Champion mendaftar program dan inisiatif, membuat kemas kini,  
dan Ketua Jabatan mengesahkan maklumat yang didaftarkan]  
```

**Jadual 20 : Definisi Aktiviti PFD-PP-HT-PR 01 Daftar Program & Inisiatif â€“ Hala Tuju**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-HT-PR |  
| Nama Fungsi | Daftar Program & Inisiatif â€“ Hala Tuju |  
| Rujukan Aktiviti | PFD-PP-HT-PR 01 |  
| Nama Aktiviti | Daftar Program & Inisiatif |  
| Keterangan Aktiviti | Mendaftar program dan inisiatif mengikut fokus dan landasan yang telah disediakan oleh Urus Setia. |  
| Aktor | Champion |  
| Tanggungjawab | Pegawai BHG/JBTN/AGENSI/UA yang dilantik oleh Ketua Jabatan masing-masing |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-HT-PR 02 Kemas kini Maklumat Program & Inisiatif |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Champion mendaftarkan program dan inisiatif berdasarkan fokus dan landasan yang telah ditetapkan oleh Urus Setia. 2\. Maklumat program dan inisiatif yang didaftarkan perlu dihantar untuk pengesahan daripada Ketua Jabatan. Sekiranya terdapat pindaan oleh Ketua Jabatan, Champion perlu melakukan proses kemas kini melalui aktiviti PFD-PP-HT-PR 02\. 3\. Maklumat yang telah dihantar untuk pengesahan hanya boleh dikemas kini sekiranya terdapat pindaan daripada Ketua Jabatan. |  
| **Penggunaan Maklumat:** | Maklumat Program dan Inisiatif 1\. Fokus Utama (R) 2\. Landasan (R) 3\. Nama Program(C) 4\. Inisiatif Strategik (C) 5\. Penerangan Program (C) 6\. KPI (C) 7\. Peruntukan (C) 8\. Tarikh Mula (C) 9\. Tarikh Tamat (C) 10\. Frekuensi Pelaporan (C) 11\. Penjajaran dengan Inisiatif KPT (C) 12\. Sasaran (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Maklumat fokus dan landasan perlu didaftarkan oleh Urus Setia sebelum Champion mendaftar maklumat program dan inisiatif. |

**Jadual 21 : Definisi Aktiviti PFD-PP-HT-PR 02 Kemas kini maklumat Program & Inisiatif**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-HT-PR |  
| Nama Fungsi | Daftar Program & Inisiatif |  
| Rujukan Aktiviti | PFD-PP-HT-PR 02 |  
| Nama Aktiviti | Kemas kini Maklumat Program & Inisiatif |  
| Keterangan Aktiviti | Mengemas kini maklumat program dan inisiatif yang telah didaftarkan. |  
| Aktor | Champion |  
| Tanggungjawab | Pegawai BHG/JBTN/AGENSI/UA yang dilantik oleh Ketua Jabatan masing-masing. |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-HT-PR 01 Daftar Program & Inisiatif |  
| Aktiviti Selepas / Aktiviti Lain | PFD-PP-HT-PR 03 Pengesahan Ketua Jabatan |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Champion mengemas kini maklumat program dan inisiatif yang telah telah disimpan dan hantar untuk pengesahan. 2\. Sekiranya terdapat permohonan pindaan daripada Ketua Jabatan semasa proses pengesahan, Champion perlu melaksanakan pengemaskinian maklumat semula. 3\. Maklumat yang telah disahkan tidak boleh dipadam atau dikemas kini. |  
| **Penggunaan Maklumat:** | Maklumat Pencapaian Program dan Inisiatif 1\. Fokus Utama (R) 2\. Landasan (R) 3\. Nama Program (RUD) 4\. Inisiatif Strategik (RUD) 5\. Penerangan Program (RUD) 6\. KPI (RUD) 7\. Peruntukan (RUD) 8\. Tarikh Mula (RUD) 9\. Tarikh Tamat (RUD) 10\. Frekuensi Pelaporan (RUD) 11\. Penjajaran dengan Inisiatif KPT (RUD) 12\. Sasaran (RUD) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 22 : Definisi Aktiviti PFD-PP-HT-PR 03 Pengesahan Ketua Jabatan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-HT-PR |  
| Nama Fungsi | Daftar Program & Inisiatif |  
| Rujukan Aktiviti | PFD-PP-HT-PR 03 |  
| Nama Aktiviti | Pengesahan Ketua Jabatan |  
| Keterangan Aktiviti | Pengesahan Ketua Jabatan berkenaan butiran program & inisiatif yang telah dikunci masuk. |  
| Aktor | Ketua Jabatan |  
| Tanggungjawab | Ketua Jabatan atau Penyelia di BHG/JBTN/AGENSI/UA |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-HT-PR 02 Kemas kini Maklumat Program & Inisiatif |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Ketua Jabatan perlu log masuk dan mengesahkan Maklumat Program & Inisiatif yang telah dikunci masuk oleh Champion. 2\. Sekiranya pengesahan tidak diluluskan, butiran Maklumat Program & Inisiatif akan dihantar ke pihak Champion untuk dikemas kini. |  
| **Penggunaan Maklumat:** | Maklumat Pencapaian Program dan Inisiatif 1\. Fokus Utama (R) 2\. Landasan (R) 3\. Nama Program (RUD) 4\. Inisiatif Strategik (RUD) 5\. Penerangan Program (RUD) 6\. KPI (RUD) 7\. Peruntukan (RUD) 8\. Tarikh Mula (RUD) 9\. Tarikh Tamat (RUD) 10\. Frekuensi Pelaporan (RUD) 11\. Penjajaran dengan Inisiatif KPT (RUD) 12\. Sasaran (RUD) 13\. Pengesahan dan Ulasan KJ (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

##### f) PFD-PP-HT-KPU Kemas Kini Pencapaian dan Ulasan Program - Hala Tuju

**Rajah 10 : Aliran Proses PFD-PP-HT-KPU Kemas kini Pencapaian dan Ulasan Program - Hala Tuju**

```  
[Rajah aliran proses menunjukkan Champion mengisi pencapaian dan ulasan, Ketua Jabatan mengesahkan,  
dan Urus setia melakukan verifikasi data]  
```

**Jadual 23 : Definisi Aktiviti PFD-PP-HT-KPU 01 Pengisian Pencapaian dan Ulasan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-HT-KPU |  
| Nama Fungsi | Kemas kini Pencapaian dan Ulasan Program |  
| Rujukan Aktiviti | PFD-PP-HT-KPU 01 |  
| Nama Aktiviti | Pengisian Pencapaian dan Ulasan |  
| Keterangan Aktiviti | Mengunci masuk atau mengemas kini pencapaian program dan ulasan program yang telah didaftarkan. |  
| Aktor | Champion |  
| Tanggungjawab | Pegawai BHG/JBTN/AGENSI/UA yang dilantik oleh Ketua Jabatan masing-masing |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-HT-KPU 02 Pengesahan Ketua Jabatan |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Champion perlu log masuk untuk mengunci masuk atau mengemas kini Pencapaian dan Ulasan Program yang telah didaftarkan. 2\. Maklumat yang telah disahkan tidak boleh dipadam atau dikemas kini. |  
| **Penggunaan Maklumat:** | Maklumat Pencapaian dan Inisiatif 1\. Fokus Utama (R) 2\. Landasan (R) 3\. Nama Program(R) 4\. Inisiatif Strategik (R) 5\. Penerangan Program (R) 6\. KPI (R) 7\. Peruntukan (R) 8\. Tarikh Mula (R) 9\. Tarikh Tamat (R) 10\. Frekuensi Pelaporan (R) 11\. Penjajaran dengan Inisiatif KPT (R) 12\. Sasaran (R) 13\. Pencapaian (CU) 14\. Ulasan (CU) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Semua aktiviti akan disimpan di dalam log bagi tujuan pengurusan. |

**Jadual 24 : Definisi Aktiviti PFD-PP-HT-KPU 02 Pengesahan Ketua Jabatan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-HT-KPU |  
| Nama Fungsi | Kemas kini Pencapaian dan Ulasan Program |  
| Rujukan Aktiviti | PFD-PP-HT-KPU 02 |  
| Nama Aktiviti | Pengesahan Ketua Jabatan |  
| Keterangan Aktiviti | Mengesahkan maklumat pencapaian dan ulasan program yang telah diisi oleh Champion. |  
| Aktor | Ketua Jabatan |  
| Tanggungjawab | Ketua Jabatan atau Penyelia di BHG/JBTN/AGENSI/UA |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-HT-KPU 01 Pengisian Pencapaian dan Ulasan |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-HT-KPU 03 Verifikasi Data |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Ketua Jabatan perlu log masuk untuk mengesahkan maklumat Pencapaian dan Ulasan Program yang telah diisi oleh Champion. 2\. Ketua Jabatan boleh memilih untuk mengesahkan atau tidak mengesahkan maklumat yang telah diisi oleh Champion. |  
| **Penggunaan Maklumat:** | Maklumat Pencapaian dan Inisiatif 1\. Fokus Utama (R) 2\. Landasan (R) 3\. Nama Program (R) 4\. Inisiatif Strategik (R) 5\. Penerangan Program (R) 6\. KPI (R) 7\. Peruntukan (R) 8\. Tarikh Mula (R) 9\. Tarikh Tamat (R) 10\. Frekuensi Pelaporan (R) 11\. Penjajaran dengan Inisiatif KPT (R) 12\. Sasaran (R) 13\. Pencapaian (R) 14\. Ulasan (R) 15\. Pengesahan dan Ulasan KJ (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Rekod yang telah disahkan perlu disimpan dan boleh diakses pada bila-bila masa. 2\. Maklumat pengesah perlu direkodkan dan disimpan. |

**Jadual 25 : Definisi Aktiviti PFD-PP-HT-KPU 03 Verifikasi Data**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-HT-KPU |  
| Nama Fungsi | Kemas kini Pencapaian dan Ulasan Program |  
| Rujukan Aktiviti | PFD-PP-HT-KPU 03 |  
| Nama Aktiviti | Verifikasi data |  
| Keterangan Aktiviti | Verifikasi data berkenaan maklumat pencapaian program yang telah disahkan oleh Ketua Jabatan. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-HT-KPU 02 Pengesahan Ketua Jabatan |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia perlu log masuk untuk menyemak maklumat Pencapaian dan Ulasan Program yang telah dihantar dan disahkan oleh Ketua Jabatan Bahagian/ Jabatan/ Agensi KPT. 2\. Urus setia boleh memilih untuk mengesahkan atau tidak mengesahkan maklumat yang telah diisi oleh Champion. 3\. Maklumat yang tidak disahkan akan diterima oleh Champion untuk dikemas kini melalui aktiviti PFD-PP-HT-KPU 01\. |  
| **Penggunaan Maklumat:** | Maklumat Pencapaian dan Ulasan Program 1\. Fokus Utama (R) 2\. Landasan (R) 3\. Nama Program (R) 4\. Inisiatif Strategik (R) 5\. Penerangan Program (R) 6\. KPI (R) 7\. Peruntukan (R) 8\. Tarikh Mula (R) 9\. Tarikh Tamat (R) 10\. Frekuensi Pelaporan (R) 11\. Penjajaran dengan Inisiatif KPT (R) 12\. Sasaran (R) 13\. Pencapaian (R) 14\. Ulasan (R) 15\. Pengesahan dan Ulasan KJ (R) 16\. Verifikasi Urus setia (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Rekod yang telah disemak perlu disimpan dan boleh diakses pada bila-bila masa. 2\. Maklumat pengesah perlu direkodkan dan disimpan. |

##### g) PFD-PP-HT-KB Kemas kini Pencapaian Keberhasilanâ€” Hala Tuju

**Rajah 11 : Aliran Proses PFD-PP-HT-KB Kemas kini Pencapaian Keberhasilan â€“ Hala Tuju**

```  
[Rajah aliran proses menunjukkan Champion mengisi pencapaian keberhasilan, Ketua Jabatan mengesahkan,  
dan Urus setia melakukan verifikasi data]  
```

**Jadual 26 : Definisi Aktiviti PFD-PP-HT-KB 01 Pengisian Pencapaian Keberhasilan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-HT-KB |  
| Nama Fungsi | Kemas kini Pencapaian Keberhasilan - Hala Tuju |  
| Rujukan Aktiviti | PFD-PP-HT-KB 01 |  
| Nama Aktiviti | Pengisian Pencapaian Keberhasilan |  
| Keterangan Aktiviti | Mengunci masuk atau mengemas kini pencapaian keberhasilan berdasarkan KPI yang telah ditetapkan. |  
| Aktor | Champion |  
| Tanggungjawab | Pegawai BHG/JBTN/AGENSI/UA yang dilantik oleh Ketua Jabatan masing-masing |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-HT-KB 02 Pengesahan Ketua Jabatan |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Champion perlu log masuk untuk mengisi pencapaian keberhasilan berdasarkan KPI dan sasaran yang telah ditetapkan. 2\. Maklumat yang telah disahkan tidak boleh dipadam atau dikemas kini. |  
| **Penggunaan Maklumat:** | Maklumat Pencapaian Keberhasilan 1\. Fokus Utama (R) 2\. KPI Fokus (R) 3\. Butiran Keberhasilan (R) 4\. Butiran Pencapaian Inisiatif (CU) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Unit ukuran adalah seperti yang telah ditetapkan oleh urus setia. 2\. Rekod yang dikunci masuk atau dikemas kini perlu disimpan dan boleh diakses pada bila-bila masa. 3\. Semua aktiviti akan disimpan di dalam log bagi tujuan pengurusan. |

**Jadual 27 : Definisi Aktiviti PFD-PP-HT-KB 02 Pengesahan Ketua Jabatan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-HT-KB |  
| Nama Fungsi | Kemas kini Pencapaian Keberhasilan - Hala Tuju |  
| Rujukan Aktiviti | PFD-PP-HT-KB 02 |  
| Nama Aktiviti | Pengesahan Ketua Jabatan |  
| Keterangan Aktiviti | Mengesahkan maklumat pencapaian keberhasilan yang telah dikunci masuk oleh Champion. |  
| Aktor | Ketua Jabatan |  
| Tanggungjawab | Ketua Jabatan atau Penyelia di BHG/JBTN/AGENSI/UA |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-HT-KB 01 Pengisian Pencapaian Keberhasilan |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-HT-KB 03 Verifikasi Data |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Ketua Jabatan perlu log masuk untuk mengesahkan maklumat pencapaian keberhasilan yang telah diisi oleh Champion. 2\. Ketua Jabatan boleh memilih untuk mengesahkan atau tidak mengesahkan maklumat yang telah diisi oleh Champion. |  
| **Penggunaan Maklumat:** | Maklumat Pencapaian Keberhasilan 1\. Fokus Utama (R) 2\. KPI Fokus (R) 3\. Butiran Keberhasilan (R) 4\. Butiran Pencapaian Inisiatif (R) 5\. Pengesahan dan Ulasan KJ (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Rekod yang telah disahkan perlu disimpan dan boleh diakses pada bila-bila masa. 2\. Maklumat pengesah perlu direkodkan dan disimpan. |

**Jadual 28 : Definisi Aktiviti PFD-PP-HT-KB 03 Verifikasi Data**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-HT-KB |  
| Nama Fungsi | Kemas kini Pencapaian Keberhasilan - Hala Tuju |  
| Rujukan Aktiviti | PFD-PP-HT-KB 03 |  
| Nama Aktiviti | Verifikasi data |  
| Keterangan Aktiviti | Verifikasi data pencapaian keberhasilan yang telah disahkan oleh Ketua Jabatan untuk disemak oleh Urus Setia. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-HT-KB 02 Pengesahan Ketua Jabatan |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia perlu log masuk untuk menyemak maklumat Pencapaian Keberhasilan yang telah dihantar dan disahkan oleh Ketua Jabatan Bahagian/ Jabatan/ Agensi KPT. 2\. Urus setia boleh memilih untuk mengesahkan atau tidak mengesahkan maklumat yang telah diisi oleh Champion. 3\. Maklumat yang tidak disahkan akan diterima oleh Champion untuk dikemas kini melalui aktiviti PFD-PP-HT-KB 01\. |  
| **Penggunaan Maklumat:** | Maklumat Pencapaian Keberhasilan 1\. Fokus Utama (R) 2\. KPI Fokus (R) 3\. Butiran Keberhasilan (R) 4\. Butiran Pencapaian Inisiatif (R) 5\. Pengesahan dan Ulasan KJ (R) 6\. Verifikasi Urus Setia (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Hala Tuju Pendidikan Tinggi |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Rekod yang telah disemak perlu disimpan dan boleh diakses pada bila-bila masa. 2\. Maklumat pengesah perlu direkodkan dan disimpan. |

##### h) PFD-PP-NRC-PSI Daftar Pencapaian dan Status Inisiatif NRC

**Rajah 12 : Aliran Proses PFD-PP-NRC-PSI Daftar Pencapaian dan Status Inisiatif NRC**

```  
[Rajah aliran proses menunjukkan Champion mengemas kini pencapaian, Ketua Jabatan mengesahkan,  
dan Urus setia melakukan verifikasi data]  
```

**Jadual 29: Definisi Aktiviti PFD-PP-NRC-PSI 01 Kemas Kini Pencapaian & Status Inisiatif**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-NRC-PSI |  
| Nama Fungsi | Daftar Pencapaian dan Status Inisiatif NRC |  
| Rujukan Aktiviti | PFD-PP-NRC-PSI 01 |  
| Nama Aktiviti | Kemas Kini Pencapaian & Status Inisiatif |  
| Keterangan Aktiviti | Mengemas kini Pencapaian dan Status Inisiatif NRC mengikut sasaran dan KPI yang telah ditetapkan. |  
| Aktor | Champion |  
| Tanggungjawab | Pegawai BHG/JBTN/AGENSI/UA |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-NRC-PSI 02 Pengesahan Ketua Jabatan |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Champion perlu log masuk untuk mengemas kini pencapaian berdasarkan maklumat NRC yang telah ditetapkan oleh urus setia. 2\. Maklumat yang telah disahkan tidak boleh dipadam atau dikemas kini. |  
| **Penggunaan Maklumat:** | Maklumat Pencapaian NRC 1\. Nama Teras (R) 2\. Nama Kategori (R) 3\. Status Inisiatif (R) 4\. Maklumat Pencapaian (CRUD) |  
| **Polisi dan Dasar Berkaitan** | 1\. Kajian Semula Dasar Pendidikan Tinggi Nasional (NRC) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Maklumat pencapaian dikemas kini mengikut tempoh masa yang telah ditetapkan oleh urus setia. 2\. Rekod yang dikemas kini perlu disimpan dan boleh diakses pada bila-bila masa. 3\. Semua aktiviti akan disimpan di dalam log bagi tujuan pengurusan. |

**Jadual 30: Definisi Aktiviti PFD-PP-NRC-PSI 02 Pengesahan Ketua Jabatan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-NRC-PSI |  
| Nama Fungsi | Daftar Pencapaian dan Status Inisiatif NRC |  
| Rujukan Aktiviti | PFD-PP-NRC-PSI 02 |  
| Nama Aktiviti | Pengesahan Ketua Jabatan |  
| Keterangan Aktiviti | Pengesahan Ketua Jabatan berkenaan butiran Pencapaian dan Status Inisiatif NRC yang telah dikunci masuk. |  
| Aktor | Ketua Jabatan |  
| Tanggungjawab | Ketua Jabatan atau Penyelia di BHG/JBTN/AGENSI/UA |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-NRC-PSI 01 Kemas Kini Pencapaian |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-NRC-PSI 03 Verifikasi Data |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Ketua Jabatan perlu log masuk untuk mengesahkan maklumat pencapaian NRC yang telah diisi oleh Champion. 2\. Ketua Jabatan boleh memilih untuk mengesahkan atau tidak mengesahkan maklumat pencapaian NRC yang telah diisi oleh Champion. |  
| **Penggunaan Maklumat:** | Maklumat Pencapaian NRC 1\. Nama Teras (R) 2\. Nama Kategori (R) 3\. Status Inisiatif (R) 4\. Maklumat Pencapaian (R) 5\. Pengesahan dan Ulasan KJ (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Kajian Semula Dasar Pendidikan Tinggi Nasional (NRC) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Rekod yang telah disahkan perlu disimpan dan boleh diakses pada bila-bila masa. 2\. Maklumat pengesah perlu direkodkan dan disimpan. |

**Jadual 31: Definisi Aktiviti PFD-PP-NRC-PSI 03 Verifikasi Data**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-NRC-PSI |  
| Nama Fungsi | Daftar Pencapaian dan Status Inisiatif NRC |  
| Rujukan Aktiviti | PFD-PP-NRC-PSI 03 |  
| Nama Aktiviti | Verifikasi data |  
| Keterangan Aktiviti | Verifikasi data berkenaan maklumat pencapaian yang telah disahkan oleh Ketua Jabatan. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-NRC-PSI 02 Pengesahan Ketua Jabatan |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia perlu log masuk untuk menyemak maklumat Pencapaian NRC yang telah dihantar dan disahkan oleh Ketua Jabatan Bahagian/ Jabatan/Agensi KPT. 2\. Urus setia boleh memilih untuk mengesahkan atau tidak mengesahkan maklumat yang telah diisi oleh Champion. 3\. Maklumat yang tidak disahkan akan diterima oleh Champion untuk dikemas kini melalui aktiviti PFD-PP-NRC-PSI 01\. |  
| **Penggunaan Maklumat:** | Maklumat Pencapaian NRC 1\. Nama Teras (R) 2\. Nama Kategori (R) 3\. Status Inisiatif (R) 4\. Maklumat Pencapaian (R) 5\. Pengesahan dan Ulasan KJ (R) 6\. Verifikasi Urus Setia (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Kajian Semula Dasar Pendidikan Tinggi Nasional (NRC) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Data yang telah disahkan oleh Ketua Jabatan hendaklah diterima oleh Urus Setia dalam tempoh 7 hari bekerja sebelum disahkan. 2\. Data yang lewat diterima dalam tempoh yang ditetapkan akan diproses pada masa berikutnya. 3\. Rekod yang telah disemak perlu disimpan dan boleh diakses pada bila-bila masa. |

##### i) PFD-PP-PM-DS Daftar Sasaran PPPM(PT)

**Rajah 13 : Aliran Proses PFD-PP-PM-DS Daftar Sasaran PPPM(PT)**

```  
[Rajah aliran proses menunjukkan Champion mendaftar sasaran, membuat kemas kini,  
dan Ketua Jabatan mengesahkan maklumat sasaran]  
```

**Jadual 32: Definisi Aktiviti PFD-PP-PM-DS 01 Daftar Sasaran**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-PM-DS |  
| Nama Fungsi | Daftar Sasaran PPPM(PT) |  
| Rujukan Aktiviti | PFD-PP-PM-DS 01 |  
| Nama Aktiviti | Daftar Sasaran |  
| Keterangan Aktiviti | Menetapkan sasaran bagi program yang telah ditetapkan oleh Urus setia. |  
| Aktor | Champion |  
| Tanggungjawab | Pegawai BHG/JBTN/AGENSI/UA yang dilantik oleh Ketua Jabatan masing-masing |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-PM-DS 02 Kemas Kini Maklumat Sasaran |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Champion perlu log masuk untuk mendaftar sasaran berdasarkan program yang telah ditetapkan oleh urus setia. 2\. Maklumat yang telah disahkan tidak boleh dipadam atau dikemas kini. |  
| **Penggunaan Maklumat:** | Maklumat PPPM(PT) 1\. Nama Lonjakan (R) 2\. Nama Strategi (R) 3\. Nama Bahagian (R) 4\. Butiran Inisiatif(R) 5\. Nama Program (R) 6\. Deskripsi (R) 7\. KPI (R) 8\. Sasaran (RUD) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Tindakan Pembangunan Pendidikan (Pendidikan Tinggi) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Maklumat sasaran dikemas kini mengikut tempoh masa yang telah ditetapkan oleh urus setia. 2\. Rekod yang didaftar perlu disimpan dan boleh diakses pada bila-bila masa. 3\. Semua aktiviti akan disimpan di dalam log bagi tujuan pengurusan. |

**Jadual 33: Definisi Aktiviti PFD-PP-PM-DS 02 Kemas Kini Maklumat Sasaran**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-PM-DS |  
| Nama Fungsi | Daftar Sasaran PPPM(PT) |  
| Rujukan Aktiviti | PFD-PP-PM-DS 02 |  
| Nama Aktiviti | Kemas Kini Maklumat Sasaran |  
| Keterangan Aktiviti | Mengemas kini maklumat sasaran yang telah disimpan atau perlu dipinda sekiranya tidak disahkan oleh Ketua Jabatan. |  
| Aktor | Champion |  
| Tanggungjawab | Pegawai BHG/JBTN/AGENSI/UA yang dilantik oleh Ketua Jabatan masing-masing |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-PM-DS 01 Daftar Sasaran |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-PM-DS 03 Pengesahan Ketua Jabatan |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Champion perlu log masuk untuk mengemas kini maklumat sasaran berdasarkan program yang telah ditetapkan oleh urus setia. 2\. Maklumat yang telah disahkan tidak boleh dipadam atau dikemas kini. |  
| **Penggunaan Maklumat:** | Maklumat PPPM(PT) 1\. Nama Lonjakan (R) 2\. Nama Strategi (R) 3\. Nama Bahagian (R) 4\. Butiran Inisiatif(R) 5\. Nama Program (R) 6\. Deskripsi (R) 7\. KPI (R) 8\. Sasaran (RUD) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Tindakan Pembangunan Pendidikan (Pendidikan Tinggi) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Maklumat yang berstatus draf boleh dikemas kini. 2\. Rekod yang dikemas kini perlu disimpan dan boleh diakses pada bila-bila masa. 3\. Semua aktiviti akan disimpan di dalam log bagi tujuan pengurusan. 4\. Maklumat sasaran dikemas kini mengikut tempoh masa yang telah ditetapkan oleh urus setia. |

**Jadual 34: Definisi Aktiviti PFD-PP-PM-DS 03 Pengesahan Ketua Jabatan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-PM-DS |  
| Nama Fungsi | Daftar Sasaran PPPM(PT) |  
| Rujukan Aktiviti | PFD-PP-PM-DS 03 |  
| Nama Aktiviti | Pengesahan Ketua Jabatan |  
| Keterangan Aktiviti | Mengesahkan maklumat sasaran program yang dihantar oleh Champion. |  
| Aktor | Ketua Jabatan |  
| Tanggungjawab | Ketua Jabatan atau Penyelia di BHG/JBTN/AGENSI/UA |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-PM-DS 01 Daftar Sasaran atau PFD-PP-PM-DS 02 Kemas Kini Maklumat Sasaran |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Ketua Jabatan perlu log masuk untuk mengesahkan maklumat sasaran PPPM(PT) yang telah diisi oleh Champion. 2\. Ketua Jabatan boleh memilih untuk mengesahkan atau tidak mengesahkan maklumat sasaran PPPM(PT) yang telah diisi oleh Champion. |  
| **Penggunaan Maklumat:** | Maklumat PPPM(PT) 1\. Nama Lonjakan (R) 2\. Nama Strategi (R) 3\. Nama Bahagian (R) 4\. Butiran Inisiatif(R) 5\. Nama Program (R) 6\. Deskripsi (R) 7\. KPI (R) 8\. Sasaran (R) 9\. Pengesahan dan Ulasan KJ (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Tindakan Pembangunan Pendidikan (Pendidikan Tinggi) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Rekod yang telah disahkan perlu disimpan dan boleh diakses pada bila-bila masa. 2\. Maklumat pengesah perlu direkodkan dan disimpan. |

##### j) PFD-PP-PM-PCI Daftar Pencapaian dan Catatan Inisiatif PPPM(PT)

**Rajah 14 : Aliran Proses PFD-PP-PM-PCI Daftar Pencapaian dan Catatan Inisiatif PPPM(PT)**

```  
[Rajah aliran proses menunjukkan Champion mengisi pencapaian, Ketua Jabatan mengesahkan,  
dan Urus setia melakukan verifikasi data]  
```

**Jadual 35: Definisi Aktiviti PFD-PP-PM-PCI 01 Pengisian Pencapaian**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-PM-PCI |  
| Nama Fungsi | Daftar Pencapaian dan Catatan Inisiatif PPPM(PT) |  
| Rujukan Aktiviti | PFD-PP-PM-PCI 01 |  
| Nama Aktiviti | Pengisian Pencapaian |  
| Keterangan Aktiviti | Mengunci masuk dan mengemas kini pencapaian mengikut sasaran dan KPI yang telah ditetapkan. |  
| Aktor | Champion |  
| Tanggungjawab | Pegawai BHG/JBTN/AGENSI/UA yang dilantik oleh Ketua Jabatan masing-masing |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-PM-PCI 02 Pengesahan Ketua Jabatan |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Champion perlu log masuk untuk mengemas kini pencapaian berdasarkan maklumat PPPM(PT) dan sasaran yang telah ditetapkan. 2\. Maklumat yang telah disahkan tidak boleh dipadam atau dikemas kini. |  
| **Penggunaan Maklumat:** | Maklumat Program 1\. Nama Lonjakan (R) 2\. Nama Strategi (R) 3\. Nama Bahagian (R) 4\. Butiran Inisiatif(R) 5\. Nama Program (R) 6\. Deskripsi (R) 7\. KPI (R) 8\. Sasaran (R) 9\. Pencapaian (CRUD) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Tindakan Pembangunan Pendidikan (Pendidikan Tinggi) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Maklumat pencapaian dikemas kini mengikut tempoh masa yang telah ditetapkan oleh urus setia. 2\. Rekod yang dikemas kini perlu disimpan dan boleh diakses pada bila-bila masa. 3\. Semua aktiviti akan disimpan di dalam log bagi tujuan pengurusan. |

**Jadual 36: Definisi Aktiviti PFD-PP-PM-PCI 02 Pengesahan Ketua Jabatan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-PM-PCI |  
| Nama Fungsi | Daftar Pencapaian dan Catatan Inisiatif PPPM(PT) |  
| Rujukan Aktiviti | PFD-PP-PM-PCI 02 |  
| Nama Aktiviti | Pengesahan Ketua Jabatan |  
| Keterangan Aktiviti | Pengesahan Ketua Jabatan berkenaan maklumat pencapaian KPI dan Catatan Inisiatif yang telah dikunci masuk. |  
| Aktor | Ketua Jabatan |  
| Tanggungjawab | Ketua Jabatan atau Penyelia di BHG/JBTN/AGENSI/UA |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-PM-PCI 01 Pengisian Pencapaian |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-PM-PCI 03 Verifikasi Data |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Ketua Jabatan perlu log masuk untuk mengesahkan maklumat pencapaian dan Catatan Inisiatif yang telah diisi oleh Champion. 2\. Ketua Jabatan boleh memilih untuk mengesahkan atau tidak mengesahkan maklumat pencapaian dan Catatan Inisiatif yang telah diisi oleh Champion. |  
| **Penggunaan Maklumat:** | Maklumat Program 1\. Nama Lonjakan (R) 2\. Nama Strategi (R) 3\. Nama Bahagian (R) 4\. Butiran Inisiatif(R) 5\. Nama Program (R) 6\. Deskripsi (R) 7\. KPI (R) 8\. Sasaran (R) 9\. Butiran Pencapaian(R) 10\. Pengesahan dan Ulasan KJ (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Tindakan Pembangunan Pendidikan (Pendidikan Tinggi) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Rekod yang telah disahkan perlu disimpan dan boleh diakses pada bila-bila masa. 2\. Maklumat pengesah perlu direkodkan dan disimpan. |

**Jadual 37: Definisi Aktiviti PFD-PP-PM-PCI 03 Verifikasi Data**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-PM-PCI |  
| Nama Fungsi | Daftar Pencapaian dan Catatan Inisiatif PPPM(PT) |  
| Rujukan Aktiviti | PFD-PP-PM-PCI 03 |  
| Nama Aktiviti | Verifikasi data |  
| Keterangan Aktiviti | Verifikasi data berkenaan maklumat pencapaian yang telah disahkan oleh Ketua Jabatan. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-PM-PCI 02 Pengesahan Ketua Jabatan |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia perlu log masuk untuk menyemak maklumat Pencapaian yang telah dihantar dan disahkan oleh Ketua Jabatan Bahagian/ Jabatan/ Agensi KPT. 2\. Urus setia boleh memilih untuk mengesahkan atau tidak mengesahkan maklumat yang telah diisi oleh Champion. 3\. Maklumat yang tidak disahkan akan diterima oleh Champion untuk dikemas kini melalui aktiviti PFD-PP-PM-PCI 01\. |  
| **Penggunaan Maklumat:** | Maklumat Pencapaian Program 1\. Nama Lonjakan (R) 2\. Nama Strategi (R) 3\. Nama Bahagian (R) 4\. Butiran Inisiatif (R) 5\. Nama Program (R) 6\. Deskripsi (R) 7\. KPI (R) 8\. Sasaran (R) 9\. Butiran Pencapaian (R) 10\. Pengesahan dan Ulasan KJ (R) 11\. Verifikasi Urus setia (CRUD) |  
| **Polisi dan Dasar Berkaitan** | 1\. Pelan Tindakan Pembangunan Pendidikan (Pendidikan Tinggi) |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Rekod yang telah disemak perlu disimpan dan boleh diakses pada bila-bila masa. 2\. Maklumat pengesah perlu direkodkan dan disimpan. |

##### k) PFD-PP-DB Papar Dashboard dan Jana Laporan

**Rajah 15 : Aliran Proses PFD-PP-DB Papar Dashboard dan Jana Laporan**

```  
[Rajah aliran proses menunjukkan Urus setia/Pengurusan Tertinggi memapar dashboard  
dan menjana laporan]  
```

**Jadual 38 : Definisi Aktiviti PFD-PP-DB 01 Papar Dashboard**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-DB |  
| Nama Fungsi | Papar Dashboard dan Jana Laporan |  
| Rujukan Aktiviti | PFD-PP-DB 01 |  
| Nama Aktiviti | Papar Dashboard |  
| Keterangan Aktiviti | Memaparkan Dashboard maklumat status rekod terkini prestasi Hala Tuju Pendidikan Tinggi. |  
| Aktor | Urus setia/Pengurusan Tertinggi |  
| Tanggungjawab | Unit HEAD/Pengurusan Tertinggi |  
| Kekerapan | 1 Hari |  
| Unit Kekerapan (Jam/Hari/Bulan) | Hari |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-DB 02 Jana Laporan |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia/Pengurusan Tertinggi perlu log masuk untuk melihat paparan dashboard. 2\. Janaan Dashboard adalah mengikut Pelan yang berstatus aktif. |  
| **Penggunaan Maklumat:** | 1\. Maklumat Pelan 2\. Maklumat Item |  
| **Polisi dan Dasar Berkaitan** | Tiada |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Dashboard dibangunkan sebagai sebahagian daripada sistem. 2\. Pembangunan dashboard menggunakan perisian Power BI KPT. 3\. Paparan data dashboard perlulah secara real-time dan mobile responsive. |

**Jadual 39 : Definisi Aktiviti PFD-PP-DB 02 Jana Laporan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-DB |  
| Nama Fungsi | Papar Dashboard dan Jana Laporan |  
| Rujukan Aktiviti | PFD-PP-DB 02 |  
| Nama Aktiviti | Jana Laporan |  
| Keterangan Aktiviti | Menjana dan memaparkan maklumat status rekod terkini pelaporan prestasi. |  
| Aktor | Urus setia/Pengurusan Tertinggi |  
| Tanggungjawab | Unit HEAD/Pengurusan Tertinggi |  
| Kekerapan | 1 Hari |  
| Unit Kekerapan (Jam/Hari/Bulan) | Hari |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia/Pengurusan Tertinggi perlu log masuk untuk menjana laporan. 2\. Janaan laporan adalah mengikut Pelan yang berstatus aktif. 3\. Urus setia/Pengurusan Tertinggi boleh memilih untuk mencetak Laporan yang dijana atau dieksport laporan untuk disimpan. |  
| **Penggunaan Maklumat:** | Maklumat Pelan (R) |  
| **Polisi dan Dasar Berkaitan** | Tiada |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Laporan dicadangkan boleh dieksport ke fail PDF atau Microsoft Excel. |

##### l) PFD-PP-AD-PG Daftar Pengguna

**Rajah 16 : Aliran Proses PFD-PP-AD-PG Daftar Pengguna**

```  
[Rajah aliran proses menunjukkan Urus setia mendaftar pengguna baru dan semua pengguna  
boleh mengemas kini profil pengguna]  
```

**Jadual 40 : Definisi Aktiviti PFD-PP-AD-PG 01 Daftar Pengguna Baru**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-AD-PG |  
| Nama Fungsi | Daftar Pengguna |  
| Rujukan Aktiviti | PFD-PP-AD-PG 01 |  
| Nama Aktiviti | Daftar Pengguna Baru |  
| Keterangan Aktiviti | Mendaftar profil pengguna baru bagi pegawai BHG/JBTN/AGENSI/UA KPT. |  
| Aktor | Urus setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-AD-PG 02 Kemas kini Profil Pengguna |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus Setia perlu log masuk untuk mendaftarkan profil pengguna. 2\. Pengguna baharu yang telah didaftarkan akan menerima notifikasi pemakluman melalui e-mel. 3\. Pengguna aktif tidak boleh dipadam. |  
| **Penggunaan Maklumat:** | Maklumat Profil Pengguna (C) |  
| **Polisi dan Dasar Berkaitan** | 1\. Polisi Keselamatan Siber KPT |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | 1\. Wujudkan ciri-ciri keselamatan pada fungsi sistem seperti pengesahan pengguna yang merangkumi kemasukan maklumat pendaftaran, daftar masuk pengguna dan lupa kata laluan. 2\. Penetapan kekuatan kata laluan dan bilangan cubaan daftar masuk selaras dengan PKS KPT sedia ada. |  
| **Catatan Tambahan:** | 1\. Semasa warga melengkapkan butiran pendaftaran perlu pastikan: â€¢ Hanya alamat e-mel rasmi agensi sahaja yang boleh didaftarkan. â€¢ Semak dan pastikan tiada pertindihan untuk kad pengenalan dan e-mel. |

**Jadual 41 : Definisi Aktiviti PFD-PP-AD-PG 02 Kemas kini Profil Pengguna**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-AD-PG |  
| Nama Fungsi | Daftar Pengguna |  
| Rujukan Aktiviti | PFD-PP-AD-PG 02 |  
| Nama Aktiviti | Kemas kini Profil Pengguna |  
| Keterangan Aktiviti | Mengemas kini maklumat profil pengguna yang berdaftar. |  
| Aktor | Semua Pengguna sistem |  
| Tanggungjawab | Semua pegawai BHG/JBTN/AGENSI/UA KPT |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-AD-PG 01 Daftar Pengguna Baru |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Pengguna baharu hanya boleh log masuk kali pertama melalui pautan pada e-mel notifikasi pemakluman yang diterima. 2\. Pengguna yang telah mendaftar boleh mengemas kini maklumat profil pengguna yang berkaitan. 3\. Profil asas pengguna seperti nombor kad pengenalan dan e-mel tidak boleh dikemas kini. 4\. Pengemaskinian profil pengguna boleh dilakukan pada bila-bila masa oleh pengguna yang telah berdaftar. |  
| **Penggunaan Maklumat:** | Maklumat Profil Pengguna (RU) |  
| **Polisi dan Dasar Berkaitan** | Tiada |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Data rujukan seperti nama bahagian, jawatan dan gred perlu ditetapkan dahulu dalam sistem supaya penggunaannya adalah standard. 2\. Rekod yang dikemas kini perlu disimpan dan boleh diakses pada bila-bila masa. |

##### m) PFD-PP-AD-PL Daftar Pelan

**Rajah 17 : Aliran Proses PFD-PP-AD-PL Daftar Pelan**

```  
[Rajah aliran proses menunjukkan Urus setia mendaftar pelan baru dan mengemas kini pelan]  
```

**Jadual 42 : Definisi Aktiviti PFD-PP-AD-PL 01 Daftar Pelan Baru**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-AD-PL |  
| Nama Fungsi | Daftar Pelan |  
| Rujukan Aktiviti | PFD-PP-AD-PL 01 |  
| Nama Aktiviti | Daftar Pelan Baru |  
| Keterangan Aktiviti | Mendaftar Pelan baru bagi pelaporan prestasi Pendidikan Tinggi. |  
| Aktor | Urus Setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-AD-PL 02 Kemas kini Pelan |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus Setia perlu log masuk untuk mendaftarkan maklumat Pelan yang baharu. |  
| **Penggunaan Maklumat:** | Maklumat Pelan (C) |  
| **Polisi dan Dasar Berkaitan** | Tiada |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 43 : Definisi Aktiviti PFD-PP-AD-PL 02 Kemas kini Pelan**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-AD-PL |  
| Nama Fungsi | Daftar Pelan |  
| Rujukan Aktiviti | PFD-PP-AD-PL 02 |  
| Nama Aktiviti | Kemas kini Pelan |  
| Keterangan Aktiviti | Mengemas kini maklumat Pelan yang berdaftar. |  
| Aktor | Urus Setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-AD-PL 01 Daftar Pelan Baru |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia perlu log masuk untuk mengemas kini Pelan yang telah didaftarkan. 2\. Hanya Pelan yang belum digunakan di mana-mana modul boleh dikemas kini dan dipadam. 3\. Maklumat Pelan yang telah digunakan boleh dinyahaktifkan sekiranya perlu. |  
| **Penggunaan Maklumat:** | Maklumat Pelan (RUD) |  
| **Polisi dan Dasar Berkaitan** | Tiada |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Maklumat Pelan yang telah digunakan di mana-mana modul tidak boleh dipadam dan dikemas kini. |

##### n) PFD-PP-AD-IT Daftar Item

**Rajah 18 : Aliran Proses PFD-PP-AD-IT Daftar Item**

```  
[Rajah aliran proses menunjukkan Urus setia mendaftar item baru dan mengemas kini item]  
```

**Jadual 44 : Definisi Aktiviti PFD-PP-AD-IT 01 Daftar Item Baru**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-AD-IT |  
| Nama Fungsi | Daftar Item |  
| Rujukan Aktiviti | PFD-PP-AD-IT 01 |  
| Nama Aktiviti | Daftar Item Baru |  
| Keterangan Aktiviti | Mendaftar Item baharu bagi Pelan Baharu yang didaftarkan. |  
| Aktor | Urus Setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | - |  
| Aktiviti Selepas/ Aktiviti Lain | PFD-PP-AD-IT 02 Kemas kini Item |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus Setia perlu log masuk untuk mendaftarkan maklumat Item yang baharu. |  
| **Penggunaan Maklumat:** | Maklumat Item 1\. Nama Pelan (R) 2\. Butiran Item (C) |  
| **Polisi dan Dasar Berkaitan** | Tiada |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | Tiada |

**Jadual 45 : Definisi Aktiviti PFD-PP-AD-IT 02 Kemas kini Item**

| | |  
|---|---|  
| **DEFINISI AKTIVITI FUNGSI BISNES** | |  
| Rujukan Fungsi | PFD-PP-AD-IT |  
| Nama Fungsi | Daftar Item |  
| Rujukan Aktiviti | PFD-PP-AD-IT 02 |  
| Nama Aktiviti | Kemas kini Item |  
| Keterangan Aktiviti | Mengemas kini maklumat Item yang berdaftar. |  
| Aktor | Urus Setia |  
| Tanggungjawab | Unit HEAD |  
| Kekerapan | - |  
| Unit Kekerapan (Jam/Hari/Bulan) | - |  
| Aktiviti Sebelum | PFD-PP-AD-IT 01 Daftar Item Baru |  
| Aktiviti Selepas/ Aktiviti Lain | - |  
| **Kaedah/Operasi (Bagaimana):** | 1\. Urus setia perlu log masuk untuk mengemas kini Item yang telah didaftarkan. 2\. Hanya Item yang belum digunakan di mana-mana modul boleh dikemas kini dan dipadam. 3\. Maklumat Item yang telah digunakan boleh dinyahaktifkan sekiranya perlu. |  
| **Penggunaan Maklumat:** | Maklumat Item 1\. Nama Pelan (R) 2\. Butiran Item (RUD) |  
| **Polisi dan Dasar Berkaitan** | Tiada |  
| **Kaedah Alternatif** | Tiada |  
| **Ciri-ciri Kualiti (Keperluan Bukan Fungsian)** | Tiada |  
| **Catatan Tambahan:** | 1\. Maklumat Item yang telah digunakan di mana-mana modul tidak boleh dipadam dan dikemas kini. |

---

## 4\. PENGIRAAN SAIZ APLIKASI

**Jadual 46 : Pengiraan Saiz Aplikasi Menggunakan Kaedah Function Point**

| | | | | | | | | | |  
|---|---|---|---|---|---|---|---|---|---|  
| **PENGIRAAN FUNCTION POINTS** | | | | | | | | | |  
| Bil. | Komponen Fungsi | Jumlah Fungsi Transaksi / Fungsi Data | Kompleksiti | | | Jumlah Saiz (FP) | | | |  
| | | | Rendah | Sederhana | Tinggi | | | | |  
| | | | Bil. | Saiz (FP) | Bil. | Saiz (FP) | Bil. | Saiz (FP) | |  
| 1 | Generic Inputs (GEI) | 5 | | | 8 | 4.4 | | | 4.4 |  
| 2 | Generic Outputs (GEO) | 5 | | | 4.9 | 5.2 | 5.4 | | |  
| 3 | Generic Queries (GEQ) | 20 | | | 3.7 | 3.9 | 4.1 | | |  
| | **Jumlah Fungsi** | **83** | | | | | | | |  
| | **Jumlah Unadjusted Function Points (UFP)** | | | | | | | **466.3** | **529.8** | **592.8** |  
| | **Value Adjusted Factor (VAF)** | | | | | | | **1** | **1** | **1** |  
| | **Jumlah Adjusted Function Points (AFP)** | | | | | | | **466.3** | **529.8** | **592.8** |

### a) ANGGARAN SAIZ APLIKASI

| | Min | ML | Max |  
|---|---|---|---|  
| TOTAL uFP FOR DATA FUNCTION (A) | 105.0 | 149.8 | 194.6 |  
| TOTAL uFP FOR TRANSACTION FUNCTION (B) | 361.3 | 380.0 | 398.2 |  
| Modul Pentadbiran | 58.5 | 61.5 | 64.5 |  
| Modul Hala Tuju | 51.1 | 53.7 | 56.3 |  
| Modul NRC | 16.9 | 17.8 | 18.6 |  
| Modul PPPM(PT) | 16.9 | 17.8 | 18.6 |  
| Modul Semakan | 46.2 | 48.6 | 51.0 |  
| Modul Pengurusan Maklumat Prestasi | 157.0 | 165.0 | 173.0 |  
| Modul Dashboard | 14.7 | 15.6 | 16.2 |  
| **TOTAL uFP (C) \= (A)+(B)** | **466.3** | **529.8** | **592.8** |  
| VAF (D) | 1.0 | 1.0 | 1.0 |  
| **TOTAL aFP (C) x (D)** | **466.3** | **529.8** | **592.8** |

### b) ANGGARAN JUMLAH KOS

| | **JUMLAH KOS** |  
|---|---|  
| \*KOS PER FP \= RM1,200.00 (COST BASED ON THE CURRENT INFLATION RATE) |  
| Min | ML | Max |  
| RM559,560.00 | RM635,760.00 | RM711,360.00 |

### c) ANGGARAN JUMLAH MANDAYS

| | **JUMLAH MANDAYS** |  
|---|---|  
| \*MANDAYS PER FP \= JUMLAH FP \* 10 JAM / 8 JAM |  
| Min | ML | Max |  
| 583 | 662 | 741 |

### d) ANGGARAN KOS MENGIKUT MODUL

| **JUMLAH KOS (Pentadbiran)** |  
|---|  
| \*KOS PER FP \= RM1,200.00 (COST BASED ON THE CURRENT INFLATION RATE) |  
| Min | ML | Max |  
| RM88,200.00 | RM99,480.00 | RM110,760.00 |

| **JUMLAH KOS (Hala Tuju)** |  
|---|  
| \*KOS PER FP \= RM1,200.00 (COST BASED ON THE CURRENT INFLATION RATE) |  
| Min | ML | Max |  
| RM79,320.00 | RM90,120.00 | RM100,920.00 |

| **JUMLAH KOS (NRC)** |  
|---|  
| \*KOS PER FP \= RM1,200.00 (COST BASED ON THE CURRENT INFLATION RATE) |  
| Min | ML | Max |  
| RM38,280.00 | RM47,040.00 | RM55,680.00 |

| **JUMLAH KOS (PPPM(PT))** |  
|---|  
| \*KOS PER FP \= RM1,200.00 (COST BASED ON THE CURRENT INFLATION RATE) |  
| Min | ML | Max |  
| RM38,280.00 | RM47,040.00 | RM55,680.00 |

| **JUMLAH KOS (Semakan)** |  
|---|  
| \*KOS PER FP \= RM1,200.00 (COST BASED ON THE CURRENT INFLATION RATE) |  
| Min | ML | Max |  
| RM73,440.00 | RM84,000.00 | RM94,560.00 |

| **JUMLAH KOS (Pengurusan Maklumat Prestasi)** |  
|---|  
| \*KOS PER FP \= RM1,200.00 (COST BASED ON THE CURRENT INFLATION RATE) |  
| Min | ML | Max |  
| RM206,400.00 | RM223,680.00 | RM240,960.00 |

| **JUMLAH KOS (Dashboard)** |  
|---|  
| \*KOS PER FP \= RM1,200.00 (COST BASED ON THE CURRENT INFLATION RATE) |  
| Min | ML | Max |  
| RM35,640.00 | RM44,400.00 | RM52,800.00 |

---

## LAMPIRAN

LAMPIRAN 1 â€“ PENGIRAAN SAIZ APLIKASI (Terperinci)

\*[Nota: Pengiraan terperinci Function Point Analysis perlu dilampirkan di sini]\*  
