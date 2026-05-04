# 🌶️ Carolina Reaper Chili Image Segmentation
**Integration of Otsu Thresholding and Morphological Operations**

---

## 📌 Deskripsi
Project ini bertujuan untuk melakukan **segmentasi citra cabai Carolina Reaper** menggunakan metode:
- **Otsu Thresholding**
- **Operasi Morfologi**

Segmentasi digunakan untuk memisahkan objek cabai dari background sebagai tahap awal dalam sistem klasifikasi tingkat kematangan.

---

## 🎯 Tujuan
- Menghasilkan segmentasi objek cabai yang akurat
- Mengurangi noise pada hasil segmentasi
- Menyediakan metode yang cepat dan dapat digunakan secara real-time

---

## ⚙️ Metode yang Digunakan

### 1. Akuisisi Citra
- Input berupa citra RGB

### 2. Ekstraksi Channel
- Menggunakan **channel merah (R)** karena memiliki kontras terbaik

### 3. Otsu Thresholding
- Mengubah citra menjadi biner (foreground & background)
- Threshold otomatis berdasarkan histogram

### 4. Operasi Morfologi
Digunakan untuk memperbaiki hasil segmentasi:
- **Dilation** → memperbesar objek
- **Imfill** → menutup lubang pada objek
- **Erosion** → menghaluskan tepi
- **Bwareaopen** → menghapus noise kecil

---

## 🔄 Alur Proses

Input Image (RGB)
↓
Red Channel Extraction
↓
Otsu Thresholding
↓
Dilation
↓
Imfill
↓
Erosion
↓
Remove Small Objects
↓
Final Segmentation


---

## 📊 Hasil
- Akurasi segmentasi: > 99%
- Waktu komputasi: < 1 detik
- Cocok untuk aplikasi real-time

---

## 💻 Teknologi yang Digunakan
- Python
- OpenCV
- NumPy
- Matplotlib
- Scikit-image
- Google Colab

---

## 🚀 Cara Menjalankan

### 1. Buka Google Colab
👉 https://colab.research.google.com/

### 2. Copy kode dari project ini

### 3. Jalankan dan upload gambar
- Upload gambar cabai
- Sistem akan otomatis memproses segmentasi

---
