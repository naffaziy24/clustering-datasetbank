
# Segmentasi Transaksi Nasabah Bank Menggunakan K-Means Clustering

## 📌 Gambaran Proyek

Proyek ini bertujuan melakukan **segmentasi transaksi nasabah bank** menggunakan algoritma **K-Means Clustering** untuk mengidentifikasi pola perilaku transaksi dan menghasilkan insight yang dapat mendukung pengambilan keputusan berbasis data.

Analisis dilakukan pada dataset transaksi perbankan berskala besar dengan lebih dari **1 juta data transaksi**, melalui tahapan **data preprocessing, exploratory data analysis (EDA), clustering, evaluasi model, dan interpretasi bisnis**.


## 🎯 Permasalahan Bisnis

Perbankan menghasilkan data transaksi dalam jumlah besar setiap hari. Namun, tanpa segmentasi yang tepat, perusahaan akan kesulitan untuk:

- Mengidentifikasi kelompok nasabah bernilai tinggi
- Menentukan strategi pemasaran yang lebih tepat sasaran
- Meningkatkan retensi pelanggan
- Memahami pola aktivitas transaksi berdasarkan karakteristik nasabah

Melalui pendekatan clustering, data transaksi dapat dikelompokkan menjadi beberapa segmen yang memiliki karakteristik serupa.

---

## 🎯 Tujuan Proyek

- Mengelompokkan data transaksi menggunakan algoritma **K-Means Clustering**
- Menentukan jumlah cluster optimal menggunakan **Elbow Method** dan **Davies–Bouldin Index (DBI)**
- Mengevaluasi performa algoritma pada dataset berukuran besar
- Menghasilkan insight yang dapat digunakan dalam strategi bisnis


## 📂 Dataset

**Sumber Data:** Kaggle – Massive Bank Dataset

### Informasi Dataset

| Keterangan | Detail |
|------------|--------|
| Total Data | 1.004.480 baris |
| Data Digunakan | 600.000 baris |
| Jenis Data | Data transaksi perbankan |
| Lokasi | India |
| Metode Analisis | Clustering |

### Variabel yang Digunakan

| Variabel | Deskripsi |
|---------|-----------|
| Date | Tanggal transaksi |
| Domain | Sektor bisnis |
| Location | Lokasi transaksi |
| Value | Total nilai transaksi |
| Transaction Count | Jumlah transaksi |


## 🛠️ Tools & Teknologi

### Bahasa Pemrograman
- Python

### Pengolahan Data
- Pandas
- NumPy

### Machine Learning
- Scikit-Learn

### Visualisasi
- Matplotlib

### Environment
- Google Colab
- Jupyter Notebook


## 🔄 Metodologi

### 1. Data Preparation
- Import dataset
- Pemeriksaan struktur data
- Identifikasi missing value dan duplikasi
- Seleksi data yang relevan

### 2. Exploratory Data Analysis (EDA)
- Analisis distribusi data
- Analisis tren transaksi
- Analisis statistik deskriptif
- Visualisasi pola transaksi

### 3. Data Preprocessing
- Pemilihan fitur:
  - Value
  - Transaction Count
- Normalisasi menggunakan **StandardScaler**

### 4. Clustering
Penerapan algoritma **K-Means Clustering**

Evaluasi dilakukan menggunakan:
- Elbow Method
- Davies–Bouldin Index (DBI)

### 5. Interpretasi Hasil
Melakukan analisis karakteristik setiap cluster untuk menghasilkan insight bisnis.


## 📊 Hasil Analisis

### Jumlah Cluster Optimal
**K = 4**

### Profil Cluster

| Cluster | Karakteristik | Interpretasi |
|----------|--------------|-------------|
| Cluster 0 | Frekuensi tinggi, nilai sedang | Nasabah aktif |
| Cluster 1 | Frekuensi rendah, nilai tinggi | Nasabah premium |
| Cluster 2 | Frekuensi tinggi, nilai tinggi | Nasabah bernilai tinggi |
| Cluster 3 | Frekuensi rendah, nilai rendah | Segmen pengembangan |


## 🔍 Insight Utama

- **Cluster 2** menjadi kelompok dengan potensi bisnis tertinggi karena memiliki frekuensi dan nilai transaksi terbesar.
- Pola segmentasi lebih dipengaruhi oleh perilaku transaksi dibanding sektor bisnis.
- Algoritma K-Means menunjukkan performa yang efisien untuk pengolahan data berskala besar.
- Distribusi cluster yang seimbang menunjukkan hasil segmentasi yang stabil.


## 📈 Evaluasi Model

| Komponen | Hasil |
|---------|-------|
| Algoritma | K-Means |
| Jumlah Cluster | 4 |
| Evaluasi | Elbow Method & DBI |
| Visualisasi | PCA |

