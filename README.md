# Ads-Click-Prediction

Ini adalah mini project yang saya dapatkan dari kaggle.com. Dataset yang saya gunakan adalah dataset Ad Click Prediction - Classification Problem yang digunakan untuk memprediksi tingkat akurasi tentang user yang akan membeli setelah mengklik iklan. 
 
 Ada pun feature-feature dalam data set ini adalah :
 1. User ID : id user
 2. Gender : Jenis kelamin user
 3. Age : usia user
 4. Estimated Salary : Jumlah gaji user
 5. Purchased : mengindikasikan user melakukan pembelian (0 = tidak; 1 = beli).



**- Exploratory Data Analysis (EDA)**

![image](https://user-images.githubusercontent.com/70499692/124575563-b4c0b480-de75-11eb-84b8-b24db90a2041.png)

Dari histogram yang sudah dibuat ini, bisa disimpulkan bahwa jumlah user yang paling banyak melakukan klik adalah yang usianya 35 tahun, disusul dengan user yang berusia 37 tahun. Jumlah user ini umumnya akan semakin berkurang untuk usia di atas 40 tahun.


![image](https://user-images.githubusercontent.com/70499692/124575734-d91c9100-de75-11eb-8d68-8b02552f852f.png)

Berdasarkan dari Grafik diatas dapat disimpulkan bahwa user yang melakukan pembelian berada di usia 40 sampai 50 tahun. Sedangkan untuk user yang tidak melakukan pembelian berada di usia 26 tahun sampai 38 tahun.


**- Preprocessing Data**

Klasifikasi Ad Click Prediction dan bagaimana cara menggunakan kNN dengan package caret di R. Caret merupakan package R yang keren banget, karena sampai saat ini sudah ada 150 algoritma machine learning yang langsung bisa kamu pakai. Caret juga sudah menyediakan function sampai contoh-contoh data (training maupun testing), preprocessing, evaluasi model, dan lain-lain.

Modelling : Logistic Regression

Model yang baik adalah model yang memiliki performa (nilai akurasi) yang baik pada saat training maupun testing. Model yang mampu
melakukan dua hal tersebut dengan baik disebut dengan Appropriate-Fitting. 


![image](https://user-images.githubusercontent.com/70499692/124577629-a5426b00-de77-11eb-82a6-bc9d93319c71.png)
![image](https://user-images.githubusercontent.com/70499692/124578884-d2dbe400-de78-11eb-88e7-832febe5b53e.png)

Berdasarkan hasil evaluasi yang sudah dilakukan, bisa disimpulkan bahwa model yang dibuat sudah sangat baik dalam memprediksi user yang akan mengklik iklan atau tidak. Hal tersebut dapat dilihat dari nilai accuracy = 1. Dimana dataset memiliki jumlah label yang seimbang (balance class), sehingga evaluasi performansi dapat menggunakan metrik Accuracy

**- Kesimpulan **

1. Exploratory Data Analysis (EDA) dapat dilakukan terhadap data numberik maupun data kategorik untuk melihat persebaran data Purchased dan tidak Purchased n dari seluruh data serta melihat persebaran data dari variable predictor lainnya terhadap label (Purchased)
2. Pembagian data menjadi 2 bagian untuk keperluan modelling (training  dan testing) pada kolom churn sama dengan persentase data di awal, hal ini mengindikasikan bahwasannya data terpisah dengan baik dan benar.
3. Logistic Regression memiliki akurasi testing 100%


