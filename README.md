# TUGAS AKUISISI DAN MANAJEMEN DATA
**Tema: Peta & Ulasan Warung Kuliner Denpasar**

## 1. Identitas Mahasiswa

- **Nama:** Renala Febrian Jono
- **NIM:** 2501010148
- **Nama:** Herkulano Yorgi Novriandri Simuk
- Nim :2501010203
- Nama:Mikael Gunawan Antul
- Nim:2501010318
- Program Studi:** Informatika
- **Mata Kuliah:** Akuisisi dan Manajemen Data

## 2. Deskripsi Proyek

Proyek ini bertujuan untuk menganalisis karakteristik data dan memperkirakan kebutuhan penyimpanan (*storage*) pada sistem peta dan ulasan warung kuliner di Denpasar.

Data yang dianalisis meliputi ulasan pelanggan, foto makanan dan warung, titik lokasi warung, serta catatan menu. Setiap jenis data memiliki format, ukuran, variasi, dan metadata yang berbeda sehingga perlu dikelola sesuai karakteristiknya.

Analisis dilakukan menggunakan Python dan library Pandas untuk mengolah data, menghitung estimasi kebutuhan penyimpanan, serta memperkirakan pertumbuhan data selama 12 bulan. Hasil analisis disimpan dalam format CSV agar mudah dibaca, diperiksa, dan digunakan kembali.

## 3. Tujuan

1. Mengidentifikasi jenis data yang dibutuhkan dalam sistem peta dan ulasan warung kuliner.
2. Menganalisis format, atribut teknis, variasi, dan metadata dari setiap jenis data.
3. Menghitung estimasi kebutuhan penyimpanan data pada bulan pertama.
4. Memperkirakan kebutuhan penyimpanan selama 12 bulan dengan asumsi pertumbuhan data sebesar 10% per bulan.
5. Menambahkan cadangan penyimpanan sebesar 30% untuk mengantisipasi pertumbuhan data dan kebutuhan operasional.
6. Menyimpan hasil analisis dalam format CSV agar dapat digunakan kembali untuk pengolahan dan evaluasi data.

## 4. Asumsi Perhitungan Storage

Perhitungan kebutuhan penyimpanan menggunakan asumsi berikut:

1. Data bulan pertama digunakan sebagai dasar perhitungan kebutuhan penyimpanan awal.
2. Jumlah data baru bertambah sebesar 10% setiap bulan dibandingkan dengan bulan sebelumnya.
3. Periode estimasi penyimpanan adalah 12 bulan.
4. Data yang telah tersimpan tetap diperhitungkan dalam akumulasi penyimpanan tahunan.
5. Cadangan penyimpanan sebesar 30% ditambahkan pada estimasi akumulasi data selama 12 bulan.
6. Konversi ukuran penyimpanan menggunakan 1 MB = 1.024 KB dan 1 GB = 1.024 MB.
7. Ukuran setiap jenis data menggunakan nilai perkiraan berdasarkan asumsi proyek, bukan hasil pengukuran langsung dari seluruh data warung kuliner di Denpasar.

Pertumbuhan data bulanan dihitung menggunakan rumus:

**Data bulan ke-n = Data bulan pertama × (1 + 10%)^(n − 1)**

Estimasi akumulasi data selama 12 bulan dihitung dengan menjumlahkan estimasi data dari bulan pertama hingga bulan kedua belas.

Kebutuhan penyimpanan akhir dihitung menggunakan rumus:

**Storage akhir = Akumulasi data 12 bulan × 130%**

Cadangan sebesar 30% digunakan untuk menyediakan ruang tambahan apabila terjadi peningkatan jumlah ulasan, foto, lokasi warung, dan catatan menu.



## 5. Metode Analisis

Analisis dilakukan menggunakan Python dengan bantuan library Pandas. Data setiap jenis objek dicatat dalam bentuk tabel yang memuat jumlah data, ukuran rata-rata, dan estimasi kebutuhan penyimpanan.

Tahapan analisis meliputi:

1. Menentukan jenis data dan asumsi jumlah data awal.
2. Menghitung kebutuhan penyimpanan bulan pertama berdasarkan jumlah data dikalikan ukuran rata-rata setiap data.
3. Menghitung pertumbuhan data sebesar 10% per bulan.
4. Menjumlahkan estimasi penyimpanan dari bulan pertama hingga bulan kedua belas.
5. Menambahkan cadangan penyimpanan sebesar 30%.
6. Mengonversi hasil perhitungan ke satuan KB, MB, atau GB sesuai kebutuhan.
7. Menyimpan hasil analisis ke dalam file CSV.

## 6. Hasil yang Diharapkan

Melalui proyek ini, diperoleh gambaran mengenai jenis dan karakteristik data yang dibutuhkan dalam sistem peta dan ulasan warung kuliner Denpasar. Proyek ini juga menghasilkan estimasi kebutuhan penyimpanan pada bulan pertama, proyeksi pertumbuhan selama 12 bulan, dan kebutuhan kapasitas akhir setelah penambahan cadangan 30%.

Hasil analisis dapat digunakan sebagai dasar perencanaan kapasitas penyimpanan agar pengelolaan data lebih terstruktur, efisien, dan mampu mengakomodasi pertumbuhan data di masa mendatang.

## 7. Kesimpulan

Analisis kebutuhan penyimpanan merupakan bagian penting dalam perancangan sistem peta dan ulasan warung kuliner. Setiap jenis data memiliki karakteristik dan kebutuhan kapasitas yang berbeda. Dengan menggunakan Python dan Pandas, estimasi penyimpanan dapat dihitung secara sistematis berdasarkan asumsi jumlah data, ukuran rata-rata, dan pertumbuhan bulanan. Penambahan cadangan 30% membantu menyediakan kapasitas tambahan untuk mendukung perkembangan sistem selama satu tahun.
