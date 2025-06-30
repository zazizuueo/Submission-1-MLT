# Submission-1-MLT

# Laporan Proyek Machine Learning - Azanti Zuhriyani

## Domain Proyek
Asuransi kesehatan menjadi salah satu sektor penting dalam kehidupan masyarakat modern, terutama dalam menanggulangi beban biaya pengobatan yang tidak terduga. Perusahaan asuransi memerlukan estimasi biaya yang akurat untuk menetapkan premi yang adil bagi pelanggan, sekaligus menjaga keberlangsungan bisnis mereka. Oleh karena itu, prediksi biaya asuransi berdasarkan karakteristik nasabah menjadi hal yang krusial. Dengan pendekatan machine learning, kita dapat membangun model prediksi biaya asuransi secara lebih objektif dan berbasis data historis yang tersedia.

## Business Understanding

### Problem Statements
1. Bagaimana memprediksi biaya asuransi kesehatan berdasarkan karakteristik nasabah seperti umur, jenis kelamin, indeks massa tubuh (BMI), jumlah anak, status merokok, dan wilayah tempat tinggal?
2. Faktor-faktor apa yang paling berpengaruh terhadap besar kecilnya biaya asuransi yang harus dibayar nasabah?

### Goals
1. Membangun model prediktif untuk memperkirakan besaran charges (biaya asuransi) berdasarkan atribut-atribut individu.
2. Mengidentifikasi fitur-fitur yang paling berkontribusi terhadap prediksi biaya asuransi untuk mendukung proses pengambilan keputusan oleh perusahaan asuransi.

    ### Solution statements
    - Mengimplementasikan model regresi yaitu, Linear Regression sebagai baseline
    - Mengukur performa model dengan metrik evaluasi R² score, Mean Absolute Error (MAE), dan Root Mean Squared Error (RMSE) untuk membandingkan akurasi prediksi.

## Data Understanding
Data yang digunakan adalah data Medical Cost Personal Datasets yang bersumber dari Kaggle (https://www.kaggle.com/datasets/mragpavank/insurance1/data). Dataset ini terdiri dari 1.338 baris dan 7 kolom yang didapatkan dari df.shape.

### Variabel-variabel pada dataset adalah sebagai berikut:
- age: umur nasabah asuransi (numerik)
- sex: jenis kelamin nasabah
- bmi: indeks massa tubuh (numerik)
- children: jumlah anak yang ditanggung (numerik)
- smoker: status merokok (kategori:yes/no)
- region: wilayah tempat tinggal
- charges: total biaya tagihan medis

## Exploratory Data Analysis
- Mengecek missing values dan duplikasi data
- Mengecek outlier dengan fungsi IQR

## Visualisasi Data
- Mengecek outlier menggunakan visualisasi boxplot
- Visualisasi Matriks Korelasi
- Visualisasi Peubah

**Rubrik/Kriteria Tambahan (Opsional)**:
- Melakukan beberapa tahapan yang diperlukan untuk memahami data, contohnya teknik visualisasi data atau exploratory data analysis.

## Data Preparation
- Encoding peubah kategorik
- Splitting data menjadi 80% data training dan 20% data testing

## Modeling
1. Linear Regression : Digunakan sebagai baseline model karena sifatnya yang sederhana dan mudah diinterpretasi.
memilih linear regression karena cepat dan mudah di interpretasikan

## Evaluation
Metrik evaluasi yang digunakan : 
- R² Score (Coefficient of Determination): Mengukur seberapa baik model menjelaskan variansi dalam data.
- MAE (Mean Absolute Error): Rata-rata selisih absolut antara prediksi dan nilai aktual.
- RMSE (Root Mean Squared Error): Menghitung akar kuadrat dari rata-rata selisih kuadrat. Lebih sensitif terhadap outlier dibanding MAE.

