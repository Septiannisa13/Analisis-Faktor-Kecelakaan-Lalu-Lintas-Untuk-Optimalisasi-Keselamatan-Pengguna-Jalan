# 🚗 **Analisis Faktor Kecelakaan Lalu Lintas untuk Optimalisasi Keselamatan Pengguna Jalan** 🚗 
📊 **Dataset:** Tersedia di [Kaggle](https://acesse.one/essTz).

## 📖 **Deskripsi Proyek**
Proyek ini bertujuan menganalisis faktor-faktor penyebab kecelakaan lalu lintas untuk meningkatkan keselamatan di jalan. Berdasarkan data Korlantas Polri, sepanjang tahun 2022 tercatat 94.617 kasus kecelakaan di Indonesia, dengan 61% di antaranya disebabkan oleh kesalahan manusia (human error). Dalam penelitian ini digunakan dataset kecelakaan lalu lintas berisi 12.316 kejadian di Sub-Kota Addis Ababa dengan 32 fitur yang merekam berbagai aspek insiden.

## 📊 **Struktur Dataset**
Dataset ini memuat beragam informasi kecelakaan lalu lintas, termasuk fitur penting seperti usia pengemudi, tingkat pendidikan, waktu kejadian, dan kondisi jalan. Target klasifikasinya terdiri dari tiga kategori cedera:

- Slight Injury – cedera ringan

- Serious Injury – cedera berat

- Fatal Injury – kecelakaan dengan korban jiwa

## 🔍 **Metodologi Proyek**
1. 🔄 **Preprocessing Data:**
- Data Cleaning: Menghapus nilai yang hilang atau tidak relevan.
- Data Reduction: Menggunakan feature selection untuk mengurangi jumlah fitur yang digunakan dalam model.
- Data Transformation: Mengonversi data kategorik menjadi numerik.
- Data Normalization: Menerapkan skala Min-Max pada data numerik agar bernilai antara 0 hingga 1.
2. ⚛️ **Algoritma Klasifikasi:**
  Model utama yang digunakan dalam analisis ini adalah Gradient Boosting Classifier, yang terbukti memberikan akurasi tinggi. Selain itu, percobaan dilakukan dengan lima algoritma lainnya untuk memastikan keakuratan model.
3. 💡 **Oversampling & Balancing:**
 Menggunakan teknik SMOTEENN untuk menangani ketidakseimbangan kelas dalam data, yang meningkatkan akurasi prediksi model.

## 📝 **Analisis Hasil**
1. Model Akurasi: Model Gradient Boosting dengan Hyperparameter Tuning menunjukkan akurasi sebesar 81%.
2. Feature Importance: Fitur Age_band_of_driver (kelompok umur pengemudi) dan Educational_level (tingkat pendidikan) menunjukkan pengaruh yang signifikan dalam menentukan tingkat keparahan kecelakaan.
3. Confusion Matrix:
- Kelas 0 (Ringan): Mengalami kesulitan dalam mengidentifikasi kasus dengan tepat.
- Kelas 1 (Sedang): Hanya 15 dari 284 kasus diprediksi dengan benar.
- Kelas 2 (Fatal): Model berhasil memprediksi 1.613 dari 2.018 kasus dengan benar.

## 📈 **Visualisasi Hasil**
Hasil analisis ditampilkan melalui Confusion Matrix dan grafik tingkat kepentingan fitur. Visualisasi ini memberikan gambaran fitur mana yang paling berperan dalam memprediksi tingkat keparahan kecelakaan.

## 📂 **Kesimpulan**
Analisis menunjukkan bahwa kesalahan manusia—terutama yang berkaitan dengan usia dan tingkat pendidikan pengemudi yang menjadi faktor utama penyebab kecelakaan lalu lintas. Temuan ini diharapkan dapat mendukung pihak berwenang dan masyarakat dalam merumuskan strategi guna meningkatkan keselamatan berkendara.
