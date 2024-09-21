# Sistem Rekomendasi [Content-based](#content-based-filtering) & [Collaborative Filtering](#collaborative-filtering)🍽️

## Content Based Filtering

Proyek ini bertujuan untuk membangun sistem rekomendasi restoran menggunakan metode Content Based Filtering berdasarkan dataset [Restaurant & Consumer Data](https://archive.ics.uci.edu/dataset/232/restaurant+consumer+data). Sistem ini akan memberikan rekomendasi restoran kepada pengguna berdasarkan jenis masakan yang mereka suka.

### Data Understanding

Dataset ini terdiri dari beberapa file CSV yang berisi informasi mengenai restoran, jenis masakan, jam buka, tempat parkir, dan rating pengguna. Berikut adalah beberapa langkah awal untuk memahami data:

1. Unduh dan Ekstrak Data
2. Baca Data ke dalam DataFrame
3. Analisis Data Melakukan analisis univariate untuk mengeksplorasi variabel yang ada, seperti jenis pembayaran yang diterima, tipe masakan, dan rating restoran.

### Data Preparation

- Menggabungkan berbagai DataFrame untuk membentuk DataFrame yang komprehensif mengenai restoran.
- Membersihkan data dari missing values dan melakukan penggabungan untuk mendapatkan informasi yang lengkap tentang restoran.

### Modeling

Model dibangun menggunakan Content Based Filtering dengan langkah-langkah sebagai berikut:

1. Representasi Data dengan TF-IDF Menggunakan `TfidfVectorizer` untuk menghitung representasi fitur dari jenis masakan.

2. Menghitung Cosine Similarity Menghitung kemiripan antara restoran menggunakan cosine similarity.

3. Fungsi Rekomendasi Membuat fungsi untuk mendapatkan rekomendasi restoran berdasarkan kemiripan.

## Collaborative Filtering

Selain Content Based Filtering, sistem ini juga menggunakan metode Collaborative Filtering dengan pendekatan neural network untuk memberikan rekomendasi yang lebih personal. Langkah-langkahnya mencakup:

1. Persiapan Data Melakukan encoding pada userID dan placeID serta membagi data menjadi set pelatihan dan validasi.

2. Pengembangan Model Neural Network Membangun model rekomendasi menggunakan TensorFlow dan Keras.

3. Visualisasi Metrik Memvisualisasikan metrik model untuk analisis performa.

### Penggunaan

1. Jalankan kode di Google Colab atau lingkungan Python yang sesuai.
2. Ikuti langkah-langkah di atas untuk membangun sistem rekomendasi.

### Catatan

Pastikan untuk menginstal semua dependensi yang diperlukan sebelum menjalankan proyek ini.
