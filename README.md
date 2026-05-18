# Tugas-EDA-Cyberpunk
Risky farel wijaya  2509116066

Latar Belakang

Dalam industri video game, khususnya pada proyek berskala besar (AAA), jumlah pemain aktif sangat dipengaruhi oleh momentum rilis, stabilitas performa, dan pembaruan konten. Salah satu contoh kasus yang paling disorot dalam beberapa tahun terakhir adalah Cyberpunk 2077 karya CD Projekt Red. Saat diluncurkan pada akhir tahun 2020, game ini berhasil mencatat rekor jumlah pemain yang sangat tinggi. Namun, tren tersebut sempat merosot tajam akibat banyaknya kendala teknis yang dialami pemain di awal rilis.
Menariknya, game ini perlahan berhasil bangkit kembali berkat perbaikan sistem yang konsisten secara berkala, perilisan ekspansi cerita (Phantom Liberty), serta dorongan popularitas dari adaptasi serial animenya. Oleh karena itu, laporan ini disusun untuk melakukan Exploratory Data Analysis (EDA) terhadap fluktuasi jumlah pemain aktif tertinggi (Peak Players) bulanan Cyberpunk 2077 di platform Steam.
Melalui analisis ini, kita dapat melihat secara lebih jelas bagaimana siklus hidup game tersebut, membandingkan tren keramaian pemain dari tahun ke tahun, serta memahami pola distribusi dan korelasi waktu terhadap naik-turunnya jumlah pemain.

 
Tahapan Proses yang Dilakukan

Proses penyelesaian analisis data ini dikerjakan secara berurutan dan dibagi ke dalam empat tahapan utama, yaitu:

A. Pengumpulan Data Data yang digunakan dalam analisis ini diambil dari dataset publik di Kaggle yang berjudul CYBERPUNK 2077 STEAM Chart - Players Over The Year.csv. Dataset ini berisi rekaman riwayat bulan, tahun, dan angka pemain tertinggi bulanan di platform Steam.

B. Persiapan dan Pembersihan Data Sebelum divisualisasikan, data mentah harus diolah terlebih dahulu menggunakan library Pandas pada bahasa pemrograman Python. Beberapa penyesuaian yang dilakukan meliputi:
•	Menghilangkan tanda baca koma (,) pada kolom jumlah pemain dan mengubah tipe datanya dari teks menjadi angka agar bisa dihitung.
•	Menyamakan format penulisan waktu menjadi standar penanggalan yang baku (datetime).
•	Menambahkan kolom spesifik untuk mengekstrak data 'Tahun' dan 'Bulan' secara terpisah guna mempermudah proses pembuatan grafik korelasi dan komposisi.

C. Analisis Data Eksploratif (EDA) Tahapan eksplorasi data divisualisasikan menggunakan empat metode utama melalui library Matplotlib dan Seaborn, yang mencakup:
•	Perbandingan (Comparison): Menggunakan diagram batang (Barplot) untuk membandingkan akumulasi Peak Players dari tahun ke tahun guna melihat tahun mana yang mencatat aktivitas pemain tertinggi.
•	Komposisi (Composition): Menggunakan diagram lingkaran (Pie Chart) untuk memetakan porsi persentase dari tiga tahun dengan kontribusi jumlah pemain paling besar.
•	Distribusi (Distribution): Menggunakan diagram Histogram untuk melihat pola persebaran jumlah pemain setiap bulannya, yang berguna untuk mengetahui apakah game ini lebih dominan berada di fase sepi atau fase ramai.

Exploratory Data Analysis (EDA)
COMPARISON / PERBANDINGAN
<img width="841" height="566" alt="{522B7488-17BE-4B40-81DA-B9B04CAD71C0}" src="https://github.com/user-attachments/assets/552a78ce-6882-4261-940b-f60da513bff4" />

COMPOSITION / KOMPOSISI
<img width="781" height="649" alt="{6388D2E0-416E-48F2-B0FC-5EF421E7D612}" src="https://github.com/user-attachments/assets/827e7ed6-2954-4921-a963-16a60275f8e6" />

DISTRIBUTION / DISTRIBUSI
<img width="838" height="542" alt="{0469B454-0068-4863-9884-F64835C26F77}" src="https://github.com/user-attachments/assets/952a599e-45d9-42f0-819f-208020f97e9a" />

RELATIONSHIP / HUBUNGAN
<img width="623" height="519" alt="{0B7126B5-46F9-4CFA-B97D-FC52B655D847}" src="https://github.com/user-attachments/assets/e1c34d4a-cc31-4863-a542-07bd7cf7c3a3" />
