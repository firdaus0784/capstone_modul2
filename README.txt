
README: Analisis Data Pengguna Transjakarta

Pendahuluan
Proyek ini bertujuan untuk menganalisis data pengguna Transjakarta guna mengidentifikasi pola perjalanan, profil demografi pengguna, dan masalah operasional seperti kegagalan tap-out dan tarif Rp 0. Analisis ini membantu Transjakarta dalam memahami perilaku pengguna, mengoptimalkan rute, dan meningkatkan sistem pembayaran melalui rekomendasi berbasis data.

Struktur Analisis
Analisis ini terdiri dari beberapa tahapan penting:
1. Persiapan Data: Membersihkan data melalui penanganan missing values, duplikasi, dan outliers.
2. Analisis Profil Pengguna: Mengidentifikasi demografi pengguna berdasarkan usia dan gender.
3. Penggunaan Kartu Pembayaran: Menganalisis distribusi jenis kartu yang digunakan serta kejadian tarif Rp 0.
4. Analisis Tap-Out yang Hilang: Mengidentifikasi kartu dan kelompok pengguna dengan masalah tap-out hilang.
5. Analisis Waktu dan Rute Perjalanan: Menentukan rute populer dan waktu puncak penggunaan layanan Transjakarta.

Dataset
Dataset mencakup data transaksi pengguna Transjakarta, yang berisi:
- Demografi Pengguna: Usia, jenis kelamin.
- Jenis Kartu Pembayaran: Nama kartu dan penyedia.
- Detail Perjalanan: Rute, waktu tap in dan tap out, serta tarif.

Langkah-Langkah Analisis

1. Penanganan Missing Values
Pendekatan imputasi digunakan untuk mengisi nilai kosong pada kolom terkait, seperti corridorID dan tapInStops, berdasarkan nilai di kolom terkait lainnya.

2. Pemeriksaan Duplikasi dan Outliers
Tidak ditemukan data duplikat dalam dataset, namun ditemukan beberapa outliers pada kolom payAmount. Outliers ini mungkin menunjukkan entri yang salah atau kasus khusus yang memerlukan investigasi lebih lanjut.

3. Profil Pengguna Berdasarkan Demografi
- Temuan: Mayoritas pengguna berusia 25-40 tahun, dengan dominasi wanita di usia produktif dan pria di usia lebih tua.
- Rekomendasi: Fokuskan layanan dan promosi pada kelompok usia produktif dan pelajar, serta tingkatkan aksesibilitas untuk lansia.

4. Penggunaan Jenis Kartu Pembayaran
- Temuan: Kartu DKI dominan digunakan di berbagai kelompok usia, terutama oleh pengguna produktif dan pelajar.
- Rekomendasi: Pertahankan kemitraan dengan Bank DKI, perluas aksesibilitas kartu untuk lansia, dan promosikan penggunaan untuk pelajar dan pekerja.

5. Kegagalan Tap-Out Berdasarkan Jenis Kartu dan Kelompok Usia
- Temuan: Kegagalan tap-out lebih tinggi pada pengguna usia <18 tahun dan >60 tahun, mungkin karena keterbatasan aksesibilitas.
- Rekomendasi: Tingkatkan edukasi terkait tap-out dan optimalkan sistem kartu dengan masalah tap-out tinggi, terutama pada kartu BNI.

6. Analisis Durasi dan Tarif Perjalanan
- Temuan: Tarif standar Rp 3,500 mendominasi, namun terdapat beberapa tarif tinggi yang mencurigakan.
- Rekomendasi: Pertimbangkan kebijakan tarif berbasis jarak dan verifikasi entri tarif tinggi.

7. Analisis Waktu dan Rute Perjalanan
- Temuan: Volume perjalanan mencapai puncak pada jam sibuk pagi dan sore di rute tertentu, seperti Kebayoran Lama - Tanah Abang dan PGC 1 - Ancol.
- Rekomendasi: Tambahkan armada pada waktu sibuk dan sesuaikan jumlah bus sesuai arah perjalanan.

Temuan Utama
- Hubungan Gender dan Rute: Uji Chi-Square menunjukkan hubungan signifikan antara gender dan rute yang dipilih.
- Durasi Perjalanan Berdasarkan Gender: Pria dan wanita menunjukkan perbedaan signifikan dalam durasi perjalanan.
- Volume Penumpang di Jam Sibuk: Volume penumpang lebih tinggi di pagi hari dibanding sore, menunjukkan kebutuhan layanan tambahan pada waktu tersebut.

Uji Statistik
Uji statistik dilakukan untuk mengukur signifikansi hubungan antara variabel:
- Chi-Square untuk Gender dan Rute: Ada hubungan signifikan.
- Mann-Whitney untuk Durasi Perjalanan Berdasarkan Gender: Durasi perjalanan berbeda signifikan antara pria dan wanita.
- Kruskal-Wallis untuk Volume Penumpang di Jam Sibuk: Volume penumpang pagi lebih tinggi daripada sore.

Visualisasi Utama
Visualisasi yang mendukung analisis ini meliputi:
- Distribusi Demografi Pengguna: Grafik batang usia dan gender.
- Penggunaan Kartu Pembayaran: Grafik batang berdasarkan jenis kartu dan kelompok usia.
- Kegagalan Tap-Out Berdasarkan Usia dan Jenis Kartu: Grafik batang persentase kegagalan tap-out.
- Distribusi Tarif Perjalanan: Histogram untuk tarif standar dan outliers.
- Pola Perjalanan Berdasarkan Waktu: Grafik garis untuk volume penumpang di jam sibuk.

Rekomendasi Manajemen
1. Optimalisasi Armada di Rute Populer: Alokasikan armada tambahan di rute padat pada waktu sibuk.
2. Peningkatan Sistem Pembayaran: Optimalkan sistem kartu BNI yang sering mengalami masalah tap-out.
3. Promosi Penggunaan Kartu DKI dan emoney: Promosikan kartu yang berkinerja baik sebagai pilihan utama pengguna.
4. Peningkatan Edukasi untuk Pengguna: Sosialisasikan proses tap-out untuk pengguna muda dan lansia.

Kesimpulan
Analisis ini memberikan wawasan penting mengenai penggunaan layanan Transjakarta, profil pengguna, dan kendala operasional. Rekomendasi yang dihasilkan diharapkan dapat membantu manajemen Transjakarta dalam pengambilan keputusan untuk meningkatkan kualitas layanan dan kepuasan pengguna.
