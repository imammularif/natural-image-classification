# 📸 Natural Image Classification using CNN

[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)](https://www.tensorflow.org/)
[![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Proyek ini adalah implementasi **Deep Learning** menggunakan arsitektur **Convolutional Neural Network (CNN)** untuk mengklasifikasikan gambar ke dalam 8 kategori berbeda. Proyek ini diselesaikan sebagai bagian dari kriteria kelulusan kursus Machine Learning.

## 📝 Deskripsi Dataset
Dataset yang digunakan adalah **Natural Images** yang mencakup 8 kategori:
* ✈️ **Airplane**
* 🚗 **Car**
* 🐱 **Cat**
* 🐶 **Dog**
* 🌸 **Flower**
* 🍎 **Fruit**
* 🏍️ **Motorbike**
* 👤 **Person**

Data dibagi secara sistematis menggunakan `split-folders` dengan rasio:
* **80%** Data Training
* **10%** Data Validation
* **10%** Data Test (Unseen Data)

## 🏗️ Arsitektur Model
Model dibangun menggunakan **TensorFlow Keras** dengan detail sebagai berikut:
1.  **Conv2D & MaxPooling2D**: Untuk ekstraksi fitur spasial dari gambar.
2.  **Dropout (0.5)**: Digunakan untuk meminimalisir risiko *overfitting*.
3.  **Flatten & Dense Layer**: Mengubah fitur menjadi vektor dan klasifikasi akhir.
4.  **Activation**: ReLU untuk layer tersembunyi dan Softmax untuk output layer (8 kelas).

## ⚙️ Preprocessing & Augmentasi
Untuk meningkatkan generalisasi model, dilakukan teknik:
- **Rescaling**: Normalisasi piksel ke rentang (0, 1).
- **Augmentasi**: `rotation_range`, `horizontal_flip`, dan `shear_range`.
- **Target Size**: Semua gambar diubah ukurannya menjadi **150x150** piksel.

## 📊 Hasil Evaluasi
Model ini berhasil mencapai performa yang solid:
- **Akurasi**: > 85% pada data Validasi dan Data Test.
- **Visualisasi**: Grafik *Loss* dan *Accuracy* disertakan di dalam notebook untuk memantau proses training secara transparan.

## 📂 Struktur Folder
```text
.
├── saved_model/      # Model dalam format SavedModel (.pb)
├── tflite/           # Model format TFLite & label.txt untuk Android/iOS
├── tfjs_model/       # Model format TensorFlow.js untuk Deployment Web
├── requirements.txt  # Daftar library pendukung
├── proyek_akhir.ipynb # Notebook utama (Proses training & evaluasi)
└── README.md         # Dokumentasi proyek
```

##🚀 Cara Menjalankan
1. Clone repositori ini:

```text
git clone [https://github.com/USERNAME_KAMU/natural-image-classification.git](https://github.com/USERNAME_KAMU/natural-image-classification.git)
```
2. Clone repositori ini:

```bash
pip install -r requirements.txt
```

3. Buka file proyek_akhir.ipynb di Google Colab atau Jupyter Notebook.


