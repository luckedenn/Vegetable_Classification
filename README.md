# 🥦 Vegetable Image Classification

Proyek ini menggunakan Convolutional Neural Network (CNN) untuk mengklasifikasikan gambar sayuran ke dalam 15 kelas berbeda. Dataset diambil dari Kaggle dan berisi lebih dari 21.000 gambar.

## ✅ Fitur
- Akurasi tinggi (>95%) pada training dan testing set
- Augmentasi data otomatis menggunakan `ImageDataGenerator`
- Model disimpan dalam 3 format:
  - **SavedModel** (untuk deployment di server/cloud)
  - **TF-Lite** (untuk mobile apps atau embedded devices)
  - **TFJS** (untuk dijalankan langsung di browser)

---

## 🧠 Arsitektur Model
Model CNN menggunakan layer berikut:
- 3x Conv2D + MaxPooling2D
- Flatten + Dense(256) + Dropout(0.5)
- Output layer dengan aktivasi softmax

---

## 📁 Struktur Direktori
```
vegetable-image-classification/
├── vegetable_model         # SavedModel format
├── vegetable_model.tflite  # TF-Lite format
├── tfjs_model              # TFJS format
├── requirements.txt
├── notebook.ipynb          # Notebook training dan evaluasi
└── README.md
```

## 📊 Evaluasi
- Akurasi Training: >96.13%
- Akurasi Validation: >95.70%
- Akurasi Testing: >98.50%

## 📌 Dataset
Dataset diambil dari Kaggle: [Vegetable Image Dataset](https://www.kaggle.com/datasets/misrakahmed/vegetable-image-dataset)
