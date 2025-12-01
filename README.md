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
