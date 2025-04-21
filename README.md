# 🥦 Klasifikasi Gambar Sayuran dengan CNN

Proyek ini bertujuan untuk membangun model klasifikasi gambar sayuran menggunakan Convolutional Neural Network (CNN) dengan akurasi tinggi. Dataset yang digunakan berisi lebih dari 21.000 gambar dengan resolusi tidak seragam dan terdiri dari 15 kelas berbeda. Model dilatih menggunakan TensorFlow dan hasil akhirnya disimpan dalam tiga format: SavedModel, TF-Lite, dan TFJS, untuk memastikan kompatibilitas lintas platform (server, mobile, dan web).

---

## ✅ Fitur Utama

- ✅ Akurasi tinggi (>95%) pada training dan testing set
- ✅ Dataset besar (>10.000 gambar)
- ✅ Terdiri dari ≥ 3 kelas (15 kelas sayuran)
- ✅ Menggunakan **Callback** (EarlyStopping, ReduceLROnPlateau)
- ✅ Simpan model ke dalam format **SavedModel**, **TF-Lite**, dan **TFJS**
- ✅ Bukti inferensi disertakan
- ✅ Gambar asli tanpa preprocessing resolusi (real-world condition)

---

## 🧠 Arsitektur Model CNN

Model menggunakan struktur layer berikut:
- Convolutional Layer (Conv2D) + MaxPooling2D (3x)
- Flatten
- Dense Layer (256 neuron) + Dropout 0.5
- Output layer: Dense dengan 15 neuron (softmax)

Optimizer: `Adam`  
Loss Function: `categorical_crossentropy`

---

