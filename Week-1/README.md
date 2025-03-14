# **Infrared Regression:**
Persamaan Matematis

1.   Mean Squared Error (MSE)

> MSE mengukur rata rata selisih kuadrat antara nilai prediksi dan nilai aktual. Nilai prediksi adalah harga barang bekas. Semakin kecil nilai MSE, semakin baik prediksi model

2.   Root Mean Squared Error (RMSE)

> RMSE adalah hasil akar dari MSE. RMSE mengukur kesalahan umum dari prediksi model. Semakin kecil nilai RMSE, semakin baik prediksi model

3.   R-Squared (R^2)

> Besaran untuk melihat proporsi varians dari variabel data yang dapat diprediksi. Semakin besar nilai R^2, semakin baik model dalam menangkap variabilitas data 

# **Income Classification:**
Metriks Evaluasi
1.   Akurasi
Besaran proporsi data yang diklasifikasikan dengan benar di antara jumlah total kasus. Rumusnya 
> *(TP+TN)/(TP+TN+FP+FN)*

2.   Presisi
Mengukur seberapa banyak prediksi positif yang benar-benar positif. Rumusnya
>  *TP/(TP+FP)*

3.   Recall
Mengukur berapa banyak positif aktual yang diidentifikasi dengan benar oleh model. Rumusnya
>  *TP/(TP+FN)*

4.   F1 Score
Rata-rata harmonik dari presisi dan recall. Rumusnya 
> 2 * (Presisi * Recall)/(Presisi+Recall)

5.   Area Under Curve (AUC)
 Mengukur kemampuan model untuk membedakan antara kelas positif dengan kelas negatif 

6.   Receiver Operating Characteristic (ROC)
Kurva yang memetakan rasio positif sejati terhadap rasio positif palsu pada berbagai parameter
# ** Metriks Terbaik: F1 Score **
Melihat datasets ('income.csv'), model ini mencoba menyelesaikan masalah klasifikasi biner. Target berupa pendapatan seseorang ≤ USD50.000 or > USD50.000. *Data tidak seimbang* karena jumlah data yang di bawah ≤ US$50K lebih banyak.

**Oleh karena itu, F1 Score adalah metrik evaluasi terbaik untuk implementasi ini:**

*   Metrik ini menyeimbangkan presisi dan perolehan, yang penting saat menangani kelas yang tidak seimbang
*   Metrik ini menghukum trade-off ekstrem antara presisi dan perolehan
*   Metrik ini menyediakan satu metrik yang memperhitungkan positif palsu dan negatif palsu



