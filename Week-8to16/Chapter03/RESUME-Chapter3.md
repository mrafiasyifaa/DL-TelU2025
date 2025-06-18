Berikut adalah format ulang **Chapter 3: Classification** agar konsisten dengan gaya Chapter 2:

---

# Chapter 3: Classification

## 🎯 Gambaran Umum

Chapter ini membahas tugas klasifikasi, yaitu memprediksi label diskrit untuk setiap instance data, seperti mengklasifikasikan email sebagai spam atau bukan, atau mengidentifikasi jenis bunga iris. Berbeda dengan regresi yang memprediksi nilai kontinu, klasifikasi memetakan input ke salah satu kelas yang telah ditentukan.

## 🧠 Algoritma Klasifikasi Umum

### • **K-Nearest Neighbors (KNN)**

Metode instance-based yang mengklasifikasikan data berdasarkan label dari tetangga terdekat di ruang fitur.

### • **Decision Trees**

Membagi data secara bertahap berdasarkan fitur-fitur tertentu untuk memisahkan kelas secara logis.

### • **Support Vector Machines (SVM)**

Mencari hyperplane optimal yang memisahkan kelas-kelas dalam ruang fitur berdimensi tinggi.

### • **Logistic Regression**

Model linier yang menggunakan fungsi sigmoid untuk menghasilkan probabilitas suatu instance masuk ke dalam kelas tertentu.

## 📏 Evaluasi Kinerja Model

### • **Confusion Matrix**

Menunjukkan jumlah prediksi benar dan salah untuk masing-masing kelas, memberikan gambaran yang rinci tentang performa klasifikasi.

### • **Akurasi**

Ukuran yang sering digunakan namun bisa menyesatkan jika data tidak seimbang.

### • **Precision, Recall, dan F1-Score**

Metrik evaluasi yang lebih informatif terutama untuk klasifikasi dengan distribusi label yang tidak seimbang.

### • **ROC Curve dan AUC**

Digunakan untuk mengevaluasi performa klasifikasi biner pada berbagai threshold, menampilkan trade-off antara true positive rate dan false positive rate.

## 🧩 Multiclass dan Multilabel Classification

### • **Multiclass Classification**

Klasifikasi dengan lebih dari dua kelas yang saling eksklusif, contohnya klasifikasi jenis bunga iris menjadi setosa, versicolor, atau virginica.

### • **Multilabel Classification**

Satu instance dapat memiliki lebih dari satu label sekaligus, seperti pengenalan wajah dengan beberapa orang dalam satu foto.

### • **Implementasi**

Biasanya dilakukan dengan mengubah masalah menjadi beberapa klasifikasi biner independen (one-vs-rest).

## 🔧 Strategi Memperbaiki Model Klasifikasi

### • **Mengatasi Overfitting**

Menggunakan teknik seperti regularisasi atau pruning (untuk decision tree) agar model tidak terlalu menyesuaikan diri pada data latih.

### • **Feature Scaling dan Transformasi Data**

Langkah penting terutama bagi algoritma sensitif terhadap skala seperti KNN dan SVM.

### • **Cross-Validation**

Digunakan untuk mengevaluasi performa model secara lebih andal dengan membagi data menjadi beberapa subset pelatihan dan validasi.

## 🧪 Praktik Klasifikasi dengan Dataset Populer

Chapter ini juga memberikan contoh penggunaan dataset populer seperti **MNIST**, yaitu kumpulan gambar digit tulisan tangan, untuk mempraktikkan proses klasifikasi end-to-end. Topik yang dibahas meliputi pipeline, preprocessing data (seperti feature scaling dan ekstraksi fitur), serta pemilihan dan evaluasi model.

---

