# 🫁 Sistem Identifikasi Penyakit Paru Berbasis Website
### Web-Based Lung Disease Identification System
**RSUD Maria Walanda Maramis — Tugas Akhir / Final Project (Skripsi)**

---

## 🇮🇩 Bahasa Indonesia

### 📌 Tentang Proyek
Proyek ini merupakan tugas akhir (skripsi) yang dikembangkan sebagai solusi atas permasalahan nyata di **RSUD Maria Walanda Maramis**, yaitu sulitnya pasien mendapatkan informasi secara cepat dan akurat terkait hasil rontgen paru-paru mereka. Proses konvensional mengharuskan pasien menunggu lama karena pemeriksaan harus dilakukan langsung oleh dokter spesialis yang terbatas jumlahnya.

Sistem ini hadir sebagai alat bantu identifikasi awal penyakit paru melalui citra rontgen (X-Ray) menggunakan teknologi *machine learning*, sehingga informasi hasil prediksi dapat tersedia lebih cepat.

---

### 🎯 Tujuan
- Mempercepat proses identifikasi awal kondisi paru-paru pasien
- Membantu tenaga medis dengan rekomendasi prediksi berbasis AI
- Memberikan akses informasi yang lebih cepat kepada pasien di rumah sakit daerah

---

### 🧠 Model Machine Learning
- **Arsitektur:** Convolutional Neural Network (CNN)
- **Bahasa Pemrograman:** Python
- **Platform Pelatihan:** Google Colaboratory
- **Jumlah Model yang Dilatih:** 5 model (fold 1 – fold 5)
- **Model Terpilih:** `modelfold2` — dipilih karena memiliki akurasi prediksi tertinggi dibandingkan model lainnya
- **Kategori / Kelas Prediksi:**
  - 🔴 Pneumonia
  - 🟡 Bronkitis
  - 🟠 Tuberkulosis (TBC)

> ⚠️ *Catatan: Jumlah kelas dibatasi tiga kategori karena ketersediaan data rontgen dari rumah sakit yang terbatas.*

---

### 🛠️ Teknologi yang Digunakan

| Komponen | Teknologi |
|---|---|
| Frontend & Backend | Flask (Python Web Framework) |
| Database | MongoDB |
| Model AI | CNN (TensorFlow / Keras) |
| Pelatihan Model | Google Colaboratory |
| Bahasa Pemrograman | Python |

---

### ⚙️ Cara Kerja Sistem
1. Petugas/pasien mengunggah gambar rontgen paru melalui dashboard website
2. Gambar diproses oleh model CNN (`modelfold2`)
3. Sistem menampilkan hasil prediksi: **Pneumonia**, **Bronkitis**, atau **Tuberkulosis**
4. Data gambar dan hasil prediksi tersimpan di database MongoDB

---

### 🏥 Implementasi
Sistem ini telah diimplementasikan dan diuji di **RSUD Maria Walanda Maramis** sebagai bagian dari penelitian tugas akhir.

---

### ⚠️ Keterbatasan
- Data pelatihan yang digunakan berasal dari dataset rontgen rumah sakit yang jumlahnya terbatas, sehingga dapat memengaruhi performa dan generalisasi model
- Model tidak memiliki mekanisme pembaruan otomatis (*retraining*) secara berkala
- Hanya mencakup tiga kelas penyakit paru

---

## 🇬🇧 English

### 📌 About the Project
This project is a final thesis (*skripsi*) developed in response to a real-world problem at **RSUD Maria Walanda Maramis** (a regional public hospital): patients experiencing long delays in receiving accurate information about their lung X-ray results. The conventional process required patients to wait for a limited number of specialist doctors to manually review each scan.

This system serves as an early-stage lung disease identification tool using chest X-ray images and machine learning, enabling faster preliminary prediction results.

---

### 🎯 Objectives
- Speed up the early identification process for patients' lung conditions
- Assist medical staff with AI-based prediction recommendations
- Improve access to timely medical information in a regional hospital setting

---

### 🧠 Machine Learning Model
- **Architecture:** Convolutional Neural Network (CNN)
- **Programming Language:** Python
- **Training Platform:** Google Colaboratory
- **Number of Models Trained:** 5 models (fold 1 – fold 5)
- **Selected Model:** `modelfold2` — chosen for achieving the highest prediction accuracy among all trained models
- **Prediction Classes:**
  - 🔴 Pneumonia
  - 🟡 Bronchitis
  - 🟠 Tuberculosis (TB)

> ⚠️ *Note: Only three disease classes were used due to limited availability of X-ray data from the hospital.*

---

### 🛠️ Tech Stack

| Component | Technology |
|---|---|
| Frontend & Backend | Flask (Python Web Framework) |
| Database | MongoDB |
| AI Model | CNN (TensorFlow / Keras) |
| Model Training | Google Colaboratory |
| Programming Language | Python |

---

### ⚙️ How It Works
1. Medical staff or patients upload a chest X-ray image via the website dashboard
2. The image is processed by the CNN model (`modelfold2`)
3. The system displays a prediction result: **Pneumonia**, **Bronchitis**, or **Tuberculosis**
4. The image and prediction result are stored in the MongoDB database

---

### 🏥 Deployment
The system was implemented and tested at **RSUD Maria Walanda Maramis** as part of the final thesis research.

---

### ⚠️ Limitations
- Training data was sourced from a limited hospital X-ray dataset, which may affect model performance and generalizability
- The model does not include an automatic retraining or update mechanism
- Currently supports only three lung disease categories

---

## 📁 Project Structure (Overview)

```
📦 lung-disease-identification/
├── 📂 model/               # Trained CNN models (modelfold1 - modelfold5)
│   └── modelfold2.h5       # Selected best-performing model
├── 📂 static/              # CSS, JS, image assets
├── 📂 templates/           # HTML templates (Flask/Jinja2)
├── 📂 uploads/             # Uploaded X-ray images
├── app.py                  # Main Flask application
├── requirements.txt        # Python dependencies
└── README.md
```

---

## 👤 Author
**Tugas Akhir / Final Thesis**
Sistem Informasi / Teknik Informatika
RSUD Maria Walanda Maramis — Studi Kasus

---

> *Proyek ini dibuat sebagai kontribusi nyata untuk meningkatkan layanan kesehatan di daerah melalui pemanfaatan teknologi kecerdasan buatan.*
>
> *This project was created as a genuine contribution to improving regional healthcare services through the application of artificial intelligence.*
