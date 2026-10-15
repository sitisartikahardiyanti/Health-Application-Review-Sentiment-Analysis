# Health-Application-Review-Sentiment-Analysis
#### Business problem: Perusahaan belum memiliki gambaran terstruktur mengenai sentimen pengguna dan aspek layanan yang paling sering dikeluhkan.

### Pertanyaan bisnis (5W + 1H)
Aspek	Pertanyaan analisis

1. What	  : Berapa proporsi ulasan positif, negatif, dan netral? Apa saja isi sentimen negatif?
2. Who	  : Bagaimana pengalaman pengguna tercermin dalam ulasan?
3. Where  : Aplikasi atau platform mana yang memiliki sentimen lebih baik, jika data mendukung perbandingan?
4. When	  : Bagaimana sentimen berubah dari waktu ke waktu?
5. Why	  : Apa keluhan atau apresiasi yang paling sering muncul?
6. How	  : Perbaikan layanan apa yang dapat diprioritaskan berdasarkan hasil analisis?

**Target akhirnya: menghasilkan dashboard yang membantu tim produk memprioritaskan perbaikan, misalnya proses pendaftaran, konsultasi dokter, pemesanan janji, atau stabilitas aplikasi.**

Catatan: aspek layanan tersebut merupakan contoh kategori yang akan kita teliti, bukan kesimpulan sebelum data dianalisis.

### Dataset
link dataset: https://data.mendeley.com/datasets/rmmmf2dp8d/2

Indonesian Telemedicine User Review Dataset
Dataset sekitar 19.680 ulasan dari tiga aplikasi telemedicine Indonesia, dengan informasi platform, nama aplikasi, rating, teks ulasan, sentimen, dan bobot kompleksitas ulasan. Tersedia label positif, netral, dan negatif.

### Dashboard Tableau
https://public.tableau.com/app/profile/siti.sartika.hardiyanti/viz/HealthApplicationSentimentAnalysis/Dashboard1#1

### Insight dari Analisis Sentimen pada Aplikasi Kesehatan
1. Berdasarkan analisis terhadap 19.460 ulasan dari Alodokter, Halodoc, dan KlikDokter, sentimen positif mendominasi ketiga aplikasi. 
2. Halodoc menunjukkan proporsi sentimen positif tertinggi sebesar 84,82%, diikuti KlikDokter sebesar 75,75% dan Alodokter sebesar 64,31%.
3. Sebaliknya, Alodokter memiliki proporsi sentimen negatif tertinggi sebesar 30,02%, sedangkan KlikDokter sebesar 19,67% dan Halodoc sebesar 14,27%. Temuan ini menunjukkan bahwa Alodokter perlu menjadi salah satu prioritas investigasi untuk memahami faktor-faktor yang memicu ketidakpuasan pengguna.
4. Hasil uji Chi-square menunjukkan adanya hubungan yang signifikan secara statistik antara nama aplikasi dan distribusi sentimen (χ² = 884,899; p < 0,001). Nilai Cramér's V sebesar 0,1508 menunjukkan bahwa kekuatan hubungan tersebut relatif kecil. Dengan demikian, terdapat perbedaan pola sentimen di antara ketiga aplikasi, meskipun besarnya hubungan secara keseluruhan tidak tergolong kuat.
5. Secara bisnis, hasil ini dapat digunakan sebagai dasar untuk mengevaluasi pengalaman pengguna, khususnya pada aplikasi dengan proporsi sentimen negatif yang lebih tinggi. 
6. Ditemukan kata dominan dalam ulasan negatif seperti konsultasi dan chat, pembayaran dan refund, waktu tunggu, serta pembelian dan pengiriman obat.
7. Analisis lanjutan terhadap isi ulasan negatif diperlukan untuk mengidentifikasi masalah utama dari setiap masing-masing aplikasi.

### Rekomendasi
- Alodokter: telusuri tema keluhan pada ulasan negatif untuk menentukan aspek layanan yang paling perlu diperbaiki.
- Halodoc: identifikasi faktor yang sering disebut dalam ulasan positif agar praktik yang diapresiasi pengguna dapat dipertahankan.
- KlikDokter: analisis tema positif dan negatif untuk menemukan peluang peningkatan pengalaman pengguna.
- Ketiga aplikasi: lakukan analisis lanjutan terhadap tema keluhan dan uji statistik pascalanjut untuk mengetahui kategori mana yang paling berkontribusi terhadap perbedaan distribusi sentimen.
