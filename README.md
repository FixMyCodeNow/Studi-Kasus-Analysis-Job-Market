# Studi-Kasus-Analysis-Job-Market
Dalam studi kasus Power BI ini, kita akan mengeksplorasi dataset lowongan pekerjaan dunia nyata untuk menemukan berbagai insight bagi sebuah perusahaan rekrutmen fiktif bernama DataSearch. Kita akan menggunakan Power Query untuk memeriksa dan membersihkan data guna mengetahui keterampilan apa saja yang paling dibutuhkan untuk posisi data scientist, data analyst, dan data engineer. Setelah itu, kita akan menggunakan DAX untuk membangun visualisasi yang informatif dari temuan tersebut. Terakhir, kita akan menggabungkan semuanya menggunakan seluruh kemampuan Power BI untuk membuat sebuah dashboard bisnis sehingga kita dapat menjawab berbagai pertanyaan dari tim DataSearch.
# Tujuan Proyek
Menyelidiki tren pasar untuk peran-peran dalam data science.
# Konteks
Sebuah perusahaan perekrutan karyawan bernama DataSearch perlu mengungkap tren pekerjaan.
# Tugas
Menemukan tren pekerjaan dan keterampilan dalam industri data science.
# Dataset
Kumpulan data fiktif yang berisi detail penting dari berbagai postingan pekerjaan. Dataset ini memiliki 25.114 lowongan pekerjaan dengan 17 kolom informasi pada setiap postingan (Judul, Tanggal, Industri, Keterampilan, dan lainnya).
Tahapan Analisis Data : 
1. Pemeriksaan Data
2. Eksplorasi Data
3. Analisis dan Visualisasi Data
4. Pembuatan Dashboard
5. Komunikasi Insight

# 1. Menganalisis Eksplanatori
<img width="349" height="438" alt="Screenshot 2025-12-01 135827" src="https://github.com/user-attachments/assets/e5b82d83-530d-4415-9f2b-6cea7a2d6bdd" />

Rata-rata Pengalaman Kerja Berdasarkan Level Posisi
Visual bar chart dan treemap konsisten menunjukkan rentang pengalaman kerja yang diharapkan untuk tiap level pekerjaan.
Rata-rata pengalaman per level:
- Executive: 14 tahun
- Director: 9 tahun
- Mid-Senior Level: 5 tahun
- Associate: 4 tahun
- Entry Level: 2 tahun
- Internship: 0 tahun (tidak memerlukan pengalaman)
Interpretasi:
Pengalaman kerja meningkat secara logis sesuai dengan jenjang posisi. Peran Executive dan Director membutuhkan pengalaman yang sangat tinggi, sedangkan Associate dan Entry menawarkan akses lebih mudah bagi kandidat baru. Data ini bermanfaat untuk kandidat memahami ekspektasi perusahaan pada setiap level senioritas.

<img width="766" height="438" alt="Screenshot 2025-12-01 140108" src="https://github.com/user-attachments/assets/dafbb70c-34d8-4df1-99b3-d4b0ad41f9ba" />

Distribusi Job Posting berdasarkan Job Title
Visual pertama memberikan gambaran jelas tentang jumlah postingan untuk tiap posisi dalam domain data.
Insight utama:
- Data Engineer merupakan posisi yang paling banyak dicari, dengan lebih dari 3.400 postingan pekerjaan.
- Data Scientist berada di urutan kedua dengan sekitar 2.000 postingan.
- Data Analyst menyusul dengan angka ±1.500 postingan.
Peran seperti Machine Learning Engineer dan Data Science Manager memiliki jumlah posting yang jauh lebih sedikit.
Interpretasi:
Temuan ini menunjukkan bahwa kebutuhan industri saat ini sangat tinggi untuk posisi Data Engineer, menandakan bahwa perusahaan lebih fokus pada pembangunan infrastruktur data, data pipeline, dan manajemen data berskala besar. Sementara itu, data scientist dan data analyst tetap memiliki permintaan signifikan, tetapi tidak setinggi kebutuhan engineer.

<img width="766" height="437" alt="Screenshot 2025-12-01 140002" src="https://github.com/user-attachments/assets/e759dc2f-db33-4956-bfd9-6d17b5d9d978" />

Tren Postingan Pekerjaan berdasarkan Level Posisi (2017–2021)

Grafik area menunjukkan perkembangan jumlah postingan dari tahun ke tahun untuk berbagai level:
Associate, Director, Entry Level, Executive, Internship, dan Mid-Senior Level.

Insight utama:
- Jumlah posting meningkat stabil sejak 2017, dengan lonjakan signifikan sekitar 2020–2021.
- Level Mid-Senior dan Associate mendominasi jumlah posting setiap tahun.
- Level Entry meningkat secara bertahap, menunjukkan bahwa perusahaan mulai membuka lebih banyak peluang untuk talenta pemula.
- Internship, Executive, dan Director tercatat sangat rendah dan relatif stabil tanpa perubahan besar.

Interpretasi:
Lonjakan di tahun 2020–2021 berpotensi dipengaruhi oleh peningkatan transformasi digital pada masa pandemi, di mana kebutuhan akan data profesional meningkat drastis. Dominasi level mid-senior menunjukkan bahwa perusahaan cenderung mencari kandidat berpengalaman untuk peran-peran strategis.

<img width="764" height="431" alt="Screenshot 2025-12-01 141341" src="https://github.com/user-attachments/assets/5a32cc08-62b3-4aef-a68a-c30758665c9d" />

Hubungan Pengalaman Kerja dan Rata-rata Gaji (per Job Title)
Grafik ini menganalisis bagaimana rata-rata gaji meningkat seiring dengan bertambahnya years of experience untuk setiap job title dalam domain data.
Insight utama dari grafik:
  1. Semua peran menunjukkan tren kenaikan gaji seiring bertambahnya pengalaman
  Garis tren (dotted lines) bergerak naik untuk seluruh job title, menandakan bahwa:
  Pengalaman adalah faktor kunci yang secara langsung meningkatkan kompensasi bagi profesional data.
  2. Job title dengan gaji tertinggi: Data Science Manager & Data Scientist
  Data Science Manager memiliki rata-rata gaji tertinggi pada hampir semua level pengalaman.
  Data Scientist mengikuti di posisi kedua, bahkan menunjukkan beberapa lonjakan signifikan pada pengalaman 7–10 tahun.
  Ini mencerminkan bahwa skill strategis, leadership, dan advanced modelling dihargai sangat tinggi.
  3. Data Engineer memiliki pola stabil dengan kenaikan gaji yang konsisten
  Gaji Data Engineer cenderung stabil dan meningkat secara linear dari tahun ke tahun.
  Hal ini menunjukkan tingginya nilai profesi yang terkait dengan pengelolaan data, ETL pipeline, dan infrastruktur modern.
  4. Data Analyst berada di rentang gaji terendah
  Gaji Data Analyst mulai dari level paling rendah dan meningkat secara bertahap.
  Meski demikian, grafik menunjukkan peningkatan nyata pada 9–10 tahun pengalaman.
  5. Machine Learning Engineer mengalami fluktuasi besar
  ML Engineer memiliki variasi gaji yang tajam, dengan beberapa titik outlier yang sangat tinggi.
Ini menunjukkan:
perbedaan perusahaan yang ekstrem (startups vs big tech), atau variasi tanggung jawab yang besar (ML ops vs research).
Interpretasi:
Secara keseluruhan, gaji tertinggi dimiliki oleh peran dengan tanggung jawab strategis dan tingkat keahlian teknis yang lebih tinggi seperti Data Science Manager dan Data Scientist. Sementara itu, Data Engineer dan ML Engineer menunjukkan pola yang kompetitif, sedangkan Data Analyst konsisten berada pada garis bawah — namun tetap meningkat seiring pengalaman.

# 2. Analisis Market Trends

<img width="765" height="436" alt="Screenshot 2025-12-01 142042" src="https://github.com/user-attachments/assets/61ed628b-f122-4b80-9dcd-31c579c90bfb" />

Tren Permintaan Keahlian Utama (Job Skills)
Analisis didasarkan pada grafik Count of Job Skills by Job Skills (Gambar 1) dan % Skill in Posting by Year (Gambar 2).
Keahlian Paling Banyak Dicari (Volume):
- Tiga keahlian yang paling sering muncul dalam lowongan pekerjaan (dengan jumlah postingan mendekati atau melebihi 3K) adalah Python, SQL, dan Cloud/AWS.
- Python dan SQL secara konsisten menjadi fondasi utama dalam analisis data dan rekayasa data.
- Layanan Cloud Computing (AWS/Azure) juga menunjukkan permintaan yang sangat tinggi, menandakan pergeseran menuju infrastruktur berbasis cloud.
Tren Tahunan (2017-2021):
- SQL dan Python menunjukkan persentase yang sangat tinggi (di atas 50%), menggarisbawahi statusnya sebagai keahlian must-have.
- Keahlian Cloud/AWS dan Azure memiliki persentase signifikan (sekitar 40%), mencerminkan adopsi cloud yang stabil dan kuat.
- Keahlian Machine Learning menunjukkan stabilitas, sedangkan Spark dan ETL memiliki persentase yang lebih rendah namun tetap relevan.

<img width="760" height="431" alt="Screenshot 2025-12-01 142148" src="https://github.com/user-attachments/assets/8bf1e9bc-c483-44a5-b722-9110b09b6523" />

Di sini, saya menggunakan DAX untuk mengidentifikasi probabilitas kemunculan keahlian tertentu dalam sebuah lowongan pekerjaan. Untuk melakukannya, kami menggunakan prinsip probabilitas dasar. Probabilitas adanya keahlian tertentu dalam sebuah iklan pekerjaan, dapat dihitung sebagai jumlah (count) dari semua postingan pekerjaan yang mengandung keahlian tersebut dibagi dengan jumlah total dari semua postingan pekerjaan. Oleh karena itu, saya membuat tiga measure (pengukuran) yang disebut Skill Count, Posting Count, dan % of Skill in Posting yang menghitung peluang yang diperlukan. Kemudian saya membuat sebuah Matriks untuk memvisualisasikan hasilnya. Saya juga menambahkan slicer, sehingga akan lebih mudah untuk memfilter keahlian tertentu.

<img width="603" height="306" alt="Screenshot 2025-12-01 142315" src="https://github.com/user-attachments/assets/31ebbaa5-f853-4263-842f-76c8025a4d83" />

Analisis Tren Keahlian dari Tahun 2017 hingga 2021
  1. Keahlian Paling Dominan (Di Atas 50%)
- SQL (Hijau Tua): Secara konsisten menjadi keahlian yang paling banyak diminta, dengan persentase di atas 50% di sepanjang tahun yang diamati. Ini menegaskan bahwa SQL adalah fundamental yang wajib dimiliki  untuk sebagian besar peran di bidang data.
- Python (Hijau Muda): Juga berada di tingkat permintaan yang sangat tinggi, stabil di atas 50%. Bersama SQL, Python membentuk duo keahlian core yang paling penting.

  2. Keahlian Infrastruktur Cloud (Sekitar 40%)
- AWS (Biru Tua), Azure (Oranye), dan Cloud (Ungu Tua): Keahlian cloud menunjukkan permintaan yang kuat dan stabil.
- AWS dan Cloud berada di rentang 40% dan menunjukkan sedikit penurunan di tahun 2018 sebelum pulih atau stabil.
- Azure stabil di kisaran 25%-30%, menjadikannya platform cloud yang penting, meskipun permintaannya sedikit di bawah AWS.

  3. Keahlian Sekunder (20% - 30%)
- Machine Learning (Kuning): Menunjukkan permintaan yang stabil di kisaran 24%-25% sepanjang periode, menunjukkan bahwa Machine Learning adalah keahlian spesialis yang konsisten dicari.
- Programming (Merah), Database (Ungu Muda), ETL (Pink): Semua keahlian ini berada di rentang 20%-22% dan menunjukkan stabilitas, mengindikasikan bahwa kemampuan dasar pemrograman, pengelolaan database, dan proses Extract, Transform, Load (ETL) adalah persyaratan standar yang terus relevan.

  4. Keahlian dengan Permintaan Lebih Rendah
- Spark (Biru Muda): Permintaannya paling rendah di antara keahlian yang terdaftar, bergerak di sekitar 18%-20%, menunjukkan bahwa ini adalah alat spesialis untuk big data processing yang tidak dibutuhkan di semua postingan.

Kesimpulan Umum: Grafik ini menunjukkan bahwa meskipun ada sedikit fluktuasi tahunan, permintaan pasar kerja untuk keahlian data bersifat sangat stabil. SQL dan Python adalah pondasi yang tak tergantikan, sementara infrastruktur cloud (terutama AWS) memiliki peran yang sangat penting dan stabil.

<img width="765" height="311" alt="Screenshot 2025-12-01 142921" src="https://github.com/user-attachments/assets/0fdc93fb-c49a-4e08-a8cc-fa4cddfe5ed9" />

Permintaan Berdasarkan Industri dan Tingkat Pengalaman
Analisis didasarkan pada Bubble Chart (Gambar 3) yang menunjukkan pengalaman yang dibutuhkan (sumbu Y) per industri (sumbu X) dan level pekerjaan (warna).
Tingkat Pengalaman (Rata-rata):
- Sebagian besar industri (seperti Financial Services, Health, Information Technology, Internet, Management Consulting) menunjukkan rata-rata pengalaman yang dibutuhkan berada di rentang 5-10 tahun (Associate dan Mid-Senior level).
- Posisi Director dan Executive secara konsisten membutuhkan pengalaman 10-15 tahun ke atas.
Fokus Industri:
- Industri Information Technology (IT), Internet, dan Staffing & Recruiting adalah beberapa industri dengan jumlah lowongan paling aktif.
- Tingkat pengalaman yang diminta untuk posisi Entry-Level (ditunjukkan oleh lingkaran ungu) tersebar di hampir semua industri pada kisaran 0-5 tahun.

Kesimpulan Cepat (Quick Takeaway):
Pasar kerja sangat didorong oleh kebutuhan akan ahli yang mahir dalam Python dan SQL, yang didukung oleh keahlian di bidang Cloud (AWS/Azure). Sebagian besar permintaan terpusat pada kandidat dengan pengalaman Menengah (Mid-Senior) yang dapat bekerja dengan infrastruktur data yang kompleks.

# 3 Membangun Dashboard

<img width="764" height="435" alt="Screenshot 2025-12-01 144804" src="https://github.com/user-attachments/assets/69c80d6a-ece3-45a3-ad7c-90906977d862" />

Jobs Overview (Ringkasan Pekerjaan)
Bagian ini memberikan gambaran umum mengenai distribusi peran pekerjaan dan persyaratan pengalaman.

Visualisasi Utama: Treemap

Tujuan: Menunjukkan volume relatif lowongan pekerjaan per Job Title (Data Engineer, Data Scientist, Data Analyst, Business Analyst, dll.) dan keahlian yang paling dominan dalam peran tersebut (diwakili oleh ukuran kotak).

Insight Cepat: Data Engineer dan Data Scientist adalah peran dengan volume postingan tertinggi. Keahlian seperti AWS, Cloud, Python, SQL, dan Azure memiliki representasi visual yang besar di dalam Treemap, menggarisbawahi relevansinya.
Metrik Kunci & Tren Pengalaman:
Posting Count Total: Terlihat total 9556 lowongan pekerjaan yang dianalisis.
- Average of Years of Experience: Nilai rata-rata pengalaman yang dibutuhkan secara keseluruhan adalah 4.49 tahun.
- Bar Chart (Average Years by Job Position Level): Menunjukkan hierarki pengalaman yang jelas:
Executive: Rata-rata 14 tahun.
Director: Rata-rata 9 tahun.
Mid-Senior Level: Rata-rata 5 tahun.
Entry Level: Rata-rata 2 tahun.
Area Chart (Count of Job Posting ID by Year): Menunjukkan pertumbuhan lowongan pekerjaan dari 2017 ke 2021, dengan peningkatan signifikan pada posisi Associate dan Mid-Senior Level di tahun-tahun akhir.

<img width="767" height="439" alt="Screenshot 2025-12-01 144953" src="https://github.com/user-attachments/assets/0c61ba3f-f0b9-425c-a88a-7480ce4a4e0c" />

Skills Overview (Ringkasan Keahlian)
Bagian ini berfokus pada permintaan keahlian, baik dari segi volume absolut maupun tren dari waktu ke waktu.

Metrik Kunci:
- Distinct Count of Job Skills: 166 keahlian unik yang teridentifikasi.
- Job Posting With Skills: Total 8561 postingan yang mengandung skill teridentifikasi.

Visualisasi Utama: Bar Chart (Count of Job Skills)
Tujuan: Menampilkan keahlian yang paling banyak diminta (Top N).
Insight Cepat: Python dan SQL menduduki puncak daftar, diikuti oleh keahlian Cloud seperti AWS dan Azure, menegaskan temuan EDA sebelumnya. Keahlian lain seperti Machine Learning, ETL, Programming, dan alat seperti Tableau/Excel juga dicantumkan.

Visualisasi Tren: Line Chart (% Skill in Posting by Year)
Tujuan: Melacak persentase kemunculan keahlian utama dari 2018 hingga 2021.
Insight Cepat: Tren SQL dan Python stabil di atas 45%. Keahlian Cloud (AWS, Azure, Cloud) stabil di kisaran 30-40%.

<img width="765" height="439" alt="Screenshot 2025-12-01 145133" src="https://github.com/user-attachments/assets/b2630633-ef0a-480d-bbbd-3cd54c79aa04" />

Company Overview (Ringkasan Perusahaan)
Bagian ini memberikan konteks tentang di mana permintaan pekerjaan berada, berdasarkan industri dan ukuran perusahaan.
Visualisasi Utama: Bubble Chart (Average of Years of Experience by Company Industry)
Tujuan: Membandingkan tingkat pengalaman yang dibutuhkan (sumbu Y) di berbagai industri (sumbu X).
Insight Cepat: Sebagian besar industri (seperti Computer Services, Financial Services, Information Technology, Internet) menunjukkan kebutuhan yang dominan pada tingkat Mid-Senior Level dan Associate (rata-rata 5-7 tahun pengalaman). Tingkat Executive/Director membutuhkan pengalaman yang jauh lebih tinggi (15+ tahun).
Filter Interaktif: Dashboard dilengkapi dengan berbagai slicer (Job Title, Job Position Level, Company Industry, Company Name, Company Size) untuk memungkinkan eksplorasi data secara real-time dan mendalam.
