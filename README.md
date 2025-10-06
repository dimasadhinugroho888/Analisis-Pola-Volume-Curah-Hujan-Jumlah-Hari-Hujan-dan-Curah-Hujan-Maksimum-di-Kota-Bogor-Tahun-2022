# 🌧️ Analisis Curah Hujan dan Intensitas Ekstrem Kota Bogor Tahun 2022

## Deskripsi Proyek

Proyek ini menyajikan analisis mendalam terhadap data Curah Hujan Bulanan di Kota Bogor sepanjang tahun 2022. Analisis berfokus pada **identifikasi pola musiman**, hubungan antara volume dan hari hujan, serta **klasifikasi risiko intensitas hujan harian maksimum** berdasarkan standar yang ditetapkan oleh BMKG.

Kode analisis dirancang untuk dieksekusi di Google Colab dan secara otomatis melakukan *feature engineering* serta visualisasi lanjutan.

---

## 📊 Dataset yang Digunakan

Data yang dianalisis mencakup 12 bulan (Januari–Desember 2022) dengan variabel utama sebagai berikut:

| Variabel | Satuan | Deskripsi |
| :--- | :--- | :--- |
| **Bulan** | - | Periode waktu dari Januari hingga Desember 2022. |
| **Volume Curah Hujan** | mm | Total curah hujan yang terjadi dalam satu bulan. |
| **Jumlah Hari Hujan** | Hari | Jumlah hari dalam sebulan yang tercatat adanya curah hujan. |
| **Curah Hujan Maksimum** | mm/Hari | Curah hujan tertinggi yang terjadi dalam kurun waktu satu hari di bulan tersebut. |
| **Rata-rata Curah Hujan Harian** | mm/Hari | (*Feature Engineering*) Tingkat intensitas hujan rata-rata per hari hujan. |
| **Kategori Intensitas MAX** | Kategori BMKG | (*Feature Engineering*) Klasifikasi *Curah Hujan Maksimum* (Ringan, Sedang, Lebat, Sangat Lebat, Ekstrem). |

### Sumber Data Resmi

* **Nama File Asli:** `Volume Curah Hujan, Jumlah Hari Hujan, dan Curah Hujan Maksimum di Kota Bogor Tahun 2022.xlsx`
* **Penyedia Data:** Pemerintah Kota Bogor via BPS/BMKG.
* **Tautan Unduhan:** [https://data.kotabogor.go.id/getdataset/volume-curah-hujan,-jumlah-hari-hujan,-dan-curah-hujan-maksimum-di-kota-bogor](https://data.kotabogor.go.id/getdataset/volume-curah-hujan,-jumlah-hari-hujan,-dan-curah-hujan-maksimum-di-kota-bogor)

---

## 🎯 Tujuan Utama Analisis

1.  **Mengklasifikasi Risiko Ekstrem:** Mengidentifikasi bulan-bulan dengan intensitas hujan harian **Sangat Lebat** atau **Ekstrem** sebagai penanda risiko bencana tinggi.
2.  **Menganalisis Hubungan Variabel:** Menggunakan **Scatter Plot** untuk memvisualisasikan korelasi antara Volume Curah Hujan dan Jumlah Hari Hujan, serta mengaitkannya dengan intensitas MAX.
3.  **Menyajikan Distribusi Risiko:** Membuat **Pie Chart** yang menunjukkan proporsi bulan berdasarkan kategori intensitas hujan harian MAX.

---

## ✨ Manfaat dan *Insight* Proyek

Hasil analisis ini memberikan *insight* yang dapat digunakan untuk perencanaan dan mitigasi:

1.  **Kesiapsiagaan Bencana:** BPBD atau otoritas setempat dapat menggunakan data klasifikasi intensitas (Pie Chart) untuk memprioritaskan bulan-bulan dalam tahun tersebut yang membutuhkan **kesiapsiagaan banjir dan longsor** ekstra.
2.  **Perencanaan Tata Ruang:** Informasi mengenai curah hujan maksimum dan intensitas harian rata-rata penting untuk **merancang kapasitas drainase** dan infrastruktur penanganan air hujan di wilayah Kota Bogor.
3.  **Evaluasi Pola Iklim:** Analisis ini menjadi dasar evaluasi pola curah hujan 2022 dibandingkan dengan rata-rata historis (jika data tambahan tersedia), membantu mengidentifikasi anomali iklim tahunan.

---

## 🛠️ Cara Menjalankan Analisis (Google Colab)

Analisis ini menggunakan *notebook* Python di Google Colab.

### Persiapan

Pastikan Anda telah mengunduh file data asli dalam format **Excel (`.xlsx`)** dari tautan yang disediakan.

### Langkah Eksekusi

1.  Buka *notebook* Google Colab baru.
2.  Salin dan tempelkan seluruh kode Python yang telah disempurnakan.
3.  Jalankan sel kode pertama. Colab akan menampilkan tombol **"Choose Files"**.
4.  Klik tombol tersebut dan **unggah file Excel `.xlsx`** Anda.
5.  Kode akan secara otomatis memproses, membersihkan, dan menampilkan:
    * Ringkasan statistik.
    * Visualisasi **Scatter Plot** volume vs. hari hujan (dengan ukuran dan warna titik berdasarkan ekstremitas).
    * Visualisasi **Pie Chart** distribusi risiko intensitas bulanan.
