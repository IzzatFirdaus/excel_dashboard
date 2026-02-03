# Dokumen Diagram — `docs/diagrams/`

Kandungan: sumber diagram yang boleh disunting dan eksport (Mermaid / PlantUML), bersama kapsyen dan alt-text dalam **Bahasa Melayu**.

Tujuan: memberikan gambaran visual terperinci bagi seni bina, aliran ETL, skema data, urutan pemprosesan, penyebaran, aspek keselamatan, dan wireframe UI untuk projek `excel_dashboard`.

Arahan ringkas:

- Gunakan editor Mermaid (VSCode extension: "Markdown Preview Mermaid Support" atau mermaid.live) untuk membuka `.mmd` fail.
- Gunakan PlantUML (VSCode extension: "PlantUML") untuk membuka `.puml` fail.
- Eksport kepada SVG (vektor) dan PNG (fallback) untuk kegunaan laporan/pembentangan.

Senarai fail dan kapsyen (Bahasa Melayu):

1. `arkitektur-tinggi.mmd`
   - Kapsyen: Rajah 1 — Arkitektur Sistem Tinggi: aliran muat naik, pemprosesan, storan, cache, dan papan pemuka.
   - Alt-text: Rajah menunjukkan komponen utama (Client, Upload Service, Antivirus, Parser, Queue, Workers, DB, Cache, BI, Monitoring) dan aliran data.

2. `aliran-etl.mmd`
   - Kapsyen: Rajah 2 — Aliran ETL: langkah Upload → Validate → Store Raw → Enqueue → Process → Transform → Load → Aggregate → Dashboard.
   - Alt-text: Carta aliran yang menerangkan setiap fasa ETL termasuk retry, dead-letter, dan audit log.

3. `er-diagram.mmd`
   - Kapsyen: Rajah 3 — Skema Data (ERD): jadual utama seperti `files`, `rows`, `datasets`, dan `metrics` serta hubungan mereka.
   - Alt-text: ERD bagi struktur penyimpanan data ekstrak dari Excel.

4. `sequence-upload.mmd`
   - Kapsyen: Rajah 4 — Urutan Proses Muat Naik hingga Paparan: event order dari pengguna ke papan pemuka.
   - Alt-text: Diagram urutan yang menunjukkan interaksi User, Server, Queue, Worker, DB, Cache, dan Dashboard.

5. `deployment.mmd`
   - Kapsyen: Rajah 5 — Model Penyebaran: perbandingan Laragon/XAMPP (Windows native) dan pilihan Docker (`docker-compose`).
   - Alt-text: Diagram yang menunjukkan servis pada host Windows dan konfigurasi kontena jika Docker digunakan.

6. `security-flow.mmd`
   - Kapsyen: Rajah 6 — Aliran Kawalan Keselamatan: langkah sanitasi, imbasan antivirus, RBAC dan jejak audit.
   - Alt-text: Carta aliran keselamatan yang menekankan sanitasi formula dan imbasan sebelum pemprosesan.

7. `wireframe-upload.mmd`
   - Kapsyen: Rajah 7 — Wireframe: sketsa halaman muat naik, pemetaan lajur, semakan validasi, dan butang pengesahan.
   - Alt-text: Sketsa susun atur antaramuka untuk proses muat naik dan semakan data.

Nota: Sila semak dan beri maklum balas; saya boleh menjana svg/png output, atau fail `draw.io`/Figma jika anda mahu wireframe lebih terperinci.
