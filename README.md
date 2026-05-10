# natural-image-classification

# Proyek Klasifikasi Gambar - Natural Images

## Deskripsi Dataset
Dataset yang digunakan adalah "Natural Images" yang terdiri dari 8 kategori gambar (airplane, car, cat, dog, flower, fruit, motorbike, dan person). Dataset telah dibagi secara sistematis menggunakan split-folders menjadi 3 bagian dengan rasio:
- 80% Data Training
- 10% Data Validation
- 10% Data Test

## Arsitektur Model
Model dibangun menggunakan TensorFlow Keras dengan arsitektur CNN:
- Conv2D & MaxPooling2D untuk ekstraksi fitur.
- Dropout (0.5) untuk mencegah overfitting.
- Dense Layer dengan aktivasi ReLU dan Softmax.

## Tahapan Preprocessing
- Rescaling (1./255).
- Augmentasi (rotation, horizontal flip, shear range).
- Target size 150x150 piksel.

## Hasil Evaluasi
Model mencapai akurasi di atas 85% pada data validasi dan data test, memenuhi seluruh kriteria wajib dan tambahan yang ditetapkan oleh Dicoding. Visualisasi Loss dan Accuracy juga telah disertakan dalam notebook.

## Struktur Folder
- `saved_model/`: Model format SavedModel.
- `tflite/`: Model TFLite & label.txt.
- `tfjs_model/`: Model format TensorFlow.js.
- `requirements.txt`: Daftar library.
- `README.md`: Dokumentasi proyek.
