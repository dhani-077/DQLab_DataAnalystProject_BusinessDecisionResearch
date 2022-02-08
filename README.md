# DQLab Data Analyst Project: Business Decision Research Overview
* Studi kasus menurunnya pelanggan yang membeli lagi ke DQLab Sport Center selama 6 bulan terakhir.
* Diberikan data transaksi dari tahun 2013 sampai dengan tahun 2019 dalam bentuk csv.
* Mengimport data csv ke dalam python environment.
* Melakukan pembersihan dan modifikasi data.
* Mendapatkan insight dari hasil visualisasi yang telah dibuat.
* Mendapatkan insight dari model dan evaluasi model yang sudah dibuat dan diuji.

## Code and Resources Used 
**Python Version:** 3.10  
**Packages:** pandas, numpy, sklearn, matplotlib, seaborn.
**Data Source:** Data Analyst Career Track Course dari [DQLab](https://dqlab.id)

## Data Cleaning
Dari data retail yang telah diberikan oleh DQLab hal pertama yang dilakukan adalah membersihkan data, dan membuat beberapa perubahan seperti:
*	Mengubah tipe data Kolom First Transaction dan Last Transaction menjadi datetime
*	Membuat kolom 'is churn' untuk mengelompokkan customer yang sudah tidak bertransaksi selama 6 bulan terakhir
*	Menghapus kolom-kolom yang tidak dibutuhkan

## Exploratory Data Analysis
Setelah melakukan Data Cleaning yang dilakukan berikutnya adalah melakukan EDA untuk bisa memvisualisasikannya. Hasil dari visualisasi inilah yang digunakan untuk membantu analisis lebih lanjut.

![alt text](https://github.com/dhani-077/DQLab_DataAnalystProject_BusinessDecisionResearch/blob/main/gambar/graph_customer_acquisition.png "Customer First Transaction")
![alt text](https://github.com/dhani-077/DQLab_DataAnalystProject_BusinessDecisionResearch/blob/main/gambar/grap_transaction_customer.png "Number of Transaction")
![alt text](https://github.com/dhani-077/DQLab_DataAnalystProject_BusinessDecisionResearch/blob/main/gambar/year_first_transaction.png "Average Transaction")
![alt text](https://github.com/dhani-077/DQLab_DataAnalystProject_BusinessDecisionResearch/blob/main/gambar/proportion_churn_by_product.png "Churn Proportion")
![alt text](https://github.com/dhani-077/DQLab_DataAnalystProject_BusinessDecisionResearch/blob/main/gambar/customer_distribution_by_count_transaction_group.png "Count Transaction Group")
![alt text](https://github.com/dhani-077/DQLab_DataAnalystProject_BusinessDecisionResearch/blob/main/gambar/customer_distribution_by_average_transaction_amount_group.png "Average Transaction Group")

## Model Building 
Untuk melakukan pemodelan, disini variable yang digunakan untuk x nya adalah "Average_Transaction_Amount", "Count_Transaction", "Year_Diff". lalu untuk variable y diambil dari kolom "is_churn". Disini dilakukan testing pemodelan dengan test size sebesar 25%.

Pemodelan yang dilakukan adalah sebagai berikut:
*	**Logistic Regression**
*	**Confusion Matrix**
![alt text](https://github.com/dhani-077/DQLab_DataAnalystProject_BusinessDecisionResearch/blob/main/gambar/confusion_matrix.png "Confusion Matrix")

## Model performance
Dari model yang sudah dibuat tadi dilakukuan pengecekan kualitas model tersebut dengan memunculkan akurasi, presisi, dan recall nya. Hasilnya adalah sebagai berikut:
* **Accuracy** : 0.66668
* **Precision** : 0.66668
* **Recall** : 0.66668
