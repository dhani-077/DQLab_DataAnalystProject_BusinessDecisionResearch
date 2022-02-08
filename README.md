# DQLab Data Analyst Project: Business Decision Research Overview
* Studi kasus menurunnya pelanggan yang membeli lagi ke DQLab Sport Center selama 6 bulan terakhir.
* Diberikan data transaksi dari tahun 2013 sampai dengan tahun 2019 dalam bentuk csv.
* Mengimport data csv ke dalam python environment.
* Melakukan pembersihan dan modifikasi data.
* Mendapatkan insight dari hasil visualisasi yang telah dibuat.
* Mendapatkan insight dari model dan evaluasi model yang sudah dibuat dan diuji.

## Code and Resources Used 
**Python Version:** 3.10  
**Packages:** pandas, numpy, sklearn, matplotlib, seaborn
**Data Source:** Data Analyst Career Track Course dari [DQLab](https://dqlab.id)

## Data Cleaning
Dari data retail yang telah diberikan oleh DQLab hal pertama yang dilakukan adalah membersihkan data, dan membuat beberapa perubahan seperti:
*	Mengubah tipe data Kolom First Transaction dan Last Transaction menjadi datetime
*	Membuat kolom 'is churn' untuk mengelompokkan customer yang sudah tidak bertransaksi selama 6 bulan terakhir
*	Menghapus kolom-kolom yang tidak dibutuhkan

## Exploratory Data Analysis
Setelah melakukan Data Cleaning yang dilakukan berikutnya adalah melakukan EDA untuk bisa memvisualisasikannya. Hasil dari visualisasi inilah yang digunakan untuk membantu analisis lebih lanjut.

## Model Building 
Untuk melakukan pemodelan, disini variable yang digunakan adalah
