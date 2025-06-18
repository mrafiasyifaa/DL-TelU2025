---

# Chapter 4: Training Models

## 🎯 Gambaran Umum

Chapter ini membahas dasar-dasar pelatihan model Machine Learning, dengan fokus awal pada **regresi linier** sebagai contoh sederhana. Pemahaman mendalam tentang cara kerja algoritma dan proses training sangat penting untuk mengoptimalkan model serta memilih hyperparameter yang tepat.

## 📐 Model Linear Regression

### • **Definisi**

Model regresi linier memprediksi nilai kontinu sebagai kombinasi linear dari fitur input ditambah bias (intercept).

### • **Parameter**

Model memiliki parameter bobot (θ) yang disesuaikan selama pelatihan untuk meminimalkan kesalahan prediksi terhadap data training.

## ⚙️ Metode Pelatihan Model

### • **Closed-form Solution (Normal Equation)**

Solusi matematis langsung untuk menghitung parameter optimal menggunakan inverse dari matriks:

* Cocok untuk dataset kecil hingga menengah.
* Tidak efisien untuk dataset besar karena komputasi invers matriks mahal.

### • **Gradient Descent (GD)**

Metode iteratif untuk mengoptimalkan parameter secara bertahap dengan menurunkan fungsi biaya:

* **Batch GD**: Menggunakan seluruh dataset setiap iterasi.
* **Stochastic GD (SGD)**: Menggunakan satu sample per iterasi.
* **Mini-batch GD**: Kombinasi keduanya, menggunakan subset kecil per iterasi.
* Metode ini lebih scalable dan fleksibel, cocok untuk model kompleks seperti neural networks.

## 🧮 Fungsi Biaya dan Optimasi

### • **Mean Squared Error (MSE)**

Fungsi biaya umum yang menghitung rata-rata kuadrat selisih antara prediksi model dan nilai aktual.

### • **Optimasi**

Gradient Descent menggunakan turunan parsial dari fungsi biaya untuk menentukan arah dan langkah penyesuaian parameter.

## 🛡️ Regularisasi

Model kompleks dapat overfitting, yaitu performa bagus di data latih tapi buruk di data baru. Untuk mengatasi ini digunakan:

### • **Ridge Regression (L2 Regularization)**

Menambahkan penalti kuadrat terhadap besar bobot agar model tidak terlalu rumit.

### • **Lasso Regression (L1 Regularization)**

Menambahkan penalti absolut bobot, yang juga membantu seleksi fitur otomatis dengan mendorong beberapa bobot menjadi nol.

## 📈 Polynomial Regression

Untuk menangani hubungan non-linear antara fitur dan target, model linier dapat diperluas dengan menambahkan fitur polinomial:

* Meningkatkan kapasitas model.
* Memperbesar risiko overfitting — maka penting digabungkan dengan regularisasi.

## 🧮 Klasifikasi Logistic dan Softmax Regression

Meskipun fokus chapter ini pada regresi, juga dikenalkan:

### • **Logistic Regression**

Digunakan untuk klasifikasi biner, memetakan output ke probabilitas menggunakan fungsi sigmoid.

### • **Softmax Regression**

Digunakan untuk klasifikasi multiclass, menggeneralisasi logistic regression menggunakan fungsi softmax.

Keduanya dapat dianggap sebagai ekstensi dari linear regression untuk tugas klasifikasi.

## 🔍 Pentingnya Memahami Proses Training

Pemahaman mendalam tentang proses pelatihan:

* Membantu debugging dan interpretasi hasil model.
* Mempermudah pemilihan algoritma yang tepat.
* Menjadi fondasi penting sebelum masuk ke topik lanjutan seperti neural networks dan deep learning.

---
