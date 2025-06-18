---

# Chapter 6: Decision Trees

## 🎯 Gambaran Umum

Decision Trees adalah algoritma Machine Learning yang sangat **fleksibel** dan dapat digunakan baik untuk **klasifikasi** maupun **regresi**. Model ini populer karena **sifatnya yang intuitif**, mudah diinterpretasikan, dan tidak memerlukan banyak preprocessing.

## 🌳 Dasar-dasar Decision Tree

### • **White Box Model**

Model ini disebut *white box* karena **struktur pohonnya dapat dibaca dan dijelaskan** dengan aturan "if-then", berbeda dengan model seperti neural networks yang bersifat black box.

### • **Algoritma CART**

Decision Tree dilatih menggunakan algoritma **CART (Classification and Regression Trees)** yang mempartisi data secara **rekursif berdasarkan fitur terbaik**.

## 🧪 Implementasi dan Visualisasi

### • **DecisionTreeClassifier**

Contoh implementasi menggunakan dataset **Iris** memperlihatkan bagaimana pohon klasifikasi bekerja dalam membagi ruang fitur.

### • **Visualisasi**

Model decision tree mudah divisualisasikan, dan batas keputusan (*decision boundary*) dapat digambarkan untuk menunjukkan bagaimana model memisahkan kelas-kelas data.

## 🧭 Decision Trees untuk Klasifikasi

### • **Prediksi Kelas**

Proses klasifikasi dilakukan dengan **menelusuri pohon dari root ke daun** berdasarkan kondisi fitur.

### • **Estimasi Probabilitas**

Selain memprediksi kelas, decision tree juga dapat memberikan **probabilitas prediksi** dengan melihat proporsi data pelatihan di daun tertentu.

## 📈 Decision Trees untuk Regresi

### • **Prediksi Nilai Numerik**

Setiap daun memprediksi **rata-rata nilai target** dari sampel pelatihan yang jatuh pada daun tersebut.

### • **Contoh Implementasi**

Contoh pada data kuadratis yang bising menunjukkan penggunaan `DecisionTreeRegressor` dengan pengaturan **max\_depth** yang bervariasi untuk menunjukkan bagaimana pembagian input space bekerja.

### • **Fungsi Biaya**

Regresi menggunakan fungsi **Mean Squared Error (MSE)** untuk mengevaluasi kualitas pembagian node.

## ✅ Kelebihan Decision Trees

* **Interpretable**: Mudah dipahami oleh manusia.
* **No Feature Scaling**: Tidak membutuhkan normalisasi atau standardisasi fitur.
* **Fleksibel**: Dapat menangani fitur **numerik maupun kategori**.
* **Cepat**: Cocok untuk dataset kecil hingga sedang.

## ⚠️ Keterbatasan Decision Trees

* **Overfitting**: Mudah mengalami overfitting jika pohon tumbuh terlalu dalam.
* **Kurang Stabil**: Perubahan kecil pada data bisa menyebabkan struktur pohon berubah drastis.
* **Kurang Akurat**: Seringkali kalah performa dibandingkan model ensemble seperti **Random Forest** atau **Gradient Boosting**.

## 🔧 Regularisasi dan Kontrol Kompleksitas

Untuk mencegah overfitting, digunakan parameter:

* **`max_depth`**: membatasi kedalaman maksimum pohon.
* **`min_samples_split`**: jumlah minimum sampel agar node dapat dipecah.
* **`min_samples_leaf`**: jumlah minimum sampel pada sebuah daun.

Pengaturan parameter ini membantu menciptakan pohon yang lebih **generalizable** terhadap data baru.

---

Chapter 6 memperkenalkan Decision Trees sebagai model yang kuat dan mudah digunakan, dengan penekanan pada interpretasi, implementasi, serta pengendalian kompleksitas untuk hasil yang lebih baik di dunia nyata.

---
