---

# Chapter 5: Support Vector Machines (SVM)

## 🎯 Gambaran Umum

Support Vector Machines (SVM) adalah algoritma Machine Learning yang kuat dan fleksibel, digunakan dalam berbagai tugas seperti klasifikasi, regresi, dan deteksi outlier. SVM sangat cocok untuk dataset kecil hingga menengah yang memiliki pola kompleks, baik linier maupun non-linier.

## 🧩 Konsep Dasar Linear SVM

### • **Large Margin Classification**

SVM bekerja dengan mencari **hyperplane** (garis pemisah) terbaik yang **memaksimalkan margin**, yaitu jarak antara hyperplane dengan data terdekat dari masing-masing kelas.

### • **Stabilitas**

Dengan margin yang besar, model lebih tahan terhadap perubahan kecil pada data — ini disebut sebagai *large margin classifier*.

### • **Contoh Visual**

Pada dataset seperti iris, SVM menghasilkan decision boundary yang berbeda dan lebih optimal dibandingkan model linier biasa.

## ⚓ Support Vectors

### • **Definisi**

Support vectors adalah data poin yang berada paling dekat dengan hyperplane dan **menentukan posisi serta orientasi hyperplane**.

### • **Sifat Sparsity**

Karena hanya support vectors yang berperan dalam menentukan model, SVM cenderung efisien dan memiliki properti sparsity.

## 🌀 Kernel Trick

### • **Masalah Non-linear**

Untuk data yang tidak dapat dipisahkan secara linear, SVM menggunakan **fungsi kernel** untuk memetakan data ke ruang berdimensi lebih tinggi.

### • **Kernel Umum**

* **RBF (Radial Basis Function)**
* **Polynomial**
* **Sigmoid**

### • **Keunggulan**

Dengan *kernel trick*, SVM bisa mempelajari batas keputusan non-linear tanpa perlu menghitung koordinat eksplisit di ruang fitur baru.

## ⚙️ Hyperparameter Penting

### • **C (Regularization Parameter)**

Mengontrol kompromi antara **margin yang lebar** dan **kesalahan klasifikasi** pada data pelatihan.

### • **γ (Gamma)**

Digunakan pada kernel seperti RBF, mengontrol **jangkauan pengaruh** dari setiap support vector:

* Gamma kecil → pengaruh luas → model lebih smooth.
* Gamma besar → pengaruh sempit → model lebih kompleks.

Pengaturan C dan gamma yang tepat penting untuk menghindari underfitting maupun overfitting.

## 🧮 Training dan Formulasi Optimasi

### • **Quadratic Programming (QP)**

Pelatihan SVM melibatkan penyelesaian masalah optimasi kuadratik, dengan formulasi primal dan dual.

### • **Formulasi Dual**

Biasanya digunakan karena lebih efisien untuk data berdimensi tinggi dan memungkinkan penggunaan fungsi kernel.

## 📤 Output Model

### • **Prediksi Kelas**

SVM memberikan output berupa prediksi kelas dan **confidence score** (jarak terhadap hyperplane).

### • **Probabilitas**

Untuk menghasilkan prediksi berbasis probabilitas, diperlukan metode tambahan seperti **Platt Scaling**.

## 🚀 Penggunaan dan Kelebihan SVM

### • **Aplikasi Umum**

* Klasifikasi teks (seperti spam detection)
* Pengenalan gambar
* Bioinformatika dan bidang medis

### • **Kelebihan**

* Efektif di ruang fitur tinggi
* Stabil dalam performa
* Cocok untuk dataset yang tidak terlalu besar
* Memerlukan preprocessing seperti **feature scaling**

## 🧪 Latihan dan Implementasi

Chapter ini diakhiri dengan latihan praktis:

* Menerapkan SVM dengan berbagai **fungsi kernel**
* Eksperimen pada dataset seperti **MNIST** (untuk klasifikasi digit) dan **California Housing** (untuk regresi)
* Melatih kemampuan dalam **tuning hyperparameter** dan mengamati dampaknya

---

Chapter 5 memberikan pemahaman menyeluruh mengenai teori dan praktik penggunaan SVM, dari konsep margin maksimal, penggunaan kernel, hingga pengaturan parameter untuk mendapatkan model yang optimal.

---
