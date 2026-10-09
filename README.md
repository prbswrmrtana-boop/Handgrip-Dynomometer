# ✊ Handgrip Dynamometer - Vision Readout System

Sistem *Computer Vision* otomatis untuk mendeteksi dan membaca hasil pengukuran kekuatan genggaman pada alat Handgrip Dynamometer. 

## ✨ Fitur Utama
- **Automated Vision Readout:** Pembacaan hasil Handgrip Dynamometer secara digital menggunakan metode *Region of Interest* (ROI) untuk fokus pada layar alat.
- **Real-time Processing:** Mengolah tangkapan video secara langsung untuk mengekstrak angka (*OCR/7-segment detection*).

## 💻 Tech Stack & Libraries
- **Bahasa Pemrograman:** Python[cite: 1]
- **Library Utama:** OpenCV (untuk pemrosesan ROI), Ultralytics[cite: 1] (jika menggunakan model deteksi AI/YOLO)
- **Perangkat Keras:** Kamera Eksternal / *Webcam*, alat Handgrip Dynamometer

## ⚙️ Cara Kerja Sistem
1. Kamera menyorot layar hasil pada Handgrip Dynamometer.
2. Program akan menetapkan *Region of Interest* (ROI) hanya pada area angka di layar[cite: 1], mengabaikan latar belakang atau *noise* di sekitarnya.
3. Gambar di dalam kotak ROI diproses (misal: *thresholding* dan *filtering*) agar angka dapat diekstrak menjadi data numerik oleh sistem.
