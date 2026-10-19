# Bank Transaction Analysis - Machine Learning Project

**Submission Akhir Belajar Machine Learning Pemula (BMLP)**  
**Nama:** Gwyneth Eunice Widjaja

---

## 📋 Deskripsi Proyek

Proyek ini merupakan submission akhir dari kursus Belajar Machine Learning Pemula yang mencakup dua pendekatan machine learning untuk menganalisis data transaksi perbankan:

1. **Clustering Analysis** - Pengelompokan pola transaksi menggunakan unsupervised learning
2. **Classification Analysis** - Prediksi kategori transaksi menggunakan supervised learning

Dataset ini menyajikan gambaran mendalam mengenai perilaku transaksi dan pola aktivitas keuangan, yang ideal untuk eksplorasi **deteksi penipuan (fraud detection)** dan **identifikasi anomali**.

---

## 📊 Dataset

Dataset mencakup **2,512 sampel data transaksi perbankan** dengan 16 fitur:

### Fitur Utama:
- **TransactionID**: ID unik untuk setiap transaksi
- **AccountID**: ID akun pelanggan
- **TransactionAmount**: Nilai transaksi dalam mata uang
- **TransactionDate**: Tanggal dan waktu transaksi
- **TransactionType**: Jenis transaksi (Credit/Debit)
- **Location**: Lokasi geografis transaksi
- **DeviceID**: ID perangkat yang digunakan
- **IP Address**: Alamat IP transaksi
- **MerchantID**: ID merchant
- **Channel**: Kanal transaksi (Online/ATM/Branch)
- **CustomerAge**: Usia pelanggan
- **CustomerOccupation**: Pekerjaan pelanggan
- **TransactionDuration**: Durasi transaksi (detik)
- **LoginAttempts**: Jumlah percobaan login
- **AccountBalance**: Saldo akun setelah transaksi
- **PreviousTransactionDate**: Tanggal transaksi sebelumnya

---

## 🎯 Tujuan Proyek

### 1. Clustering Analysis
- Mengelompokkan transaksi berdasarkan pola perilaku
- Mengidentifikasi segmen pelanggan berdasarkan karakteristik transaksi
- Menggunakan K-Means Clustering dengan optimasi menggunakan Elbow Method
- Implementasi PCA untuk dimensionality reduction

### 2. Classification Analysis
- Membangun model prediksi untuk mengklasifikasikan kategori transaksi
- Membandingkan performa berbagai algoritma:
  - Decision Tree
  - Random Forest
  - Model dengan Hyperparameter Tuning
- Evaluasi model menggunakan metrik akurasi dan confusion matrix

---

## 🛠️ Teknologi & Library

```python
- Python 3.x
- pandas - Data manipulation
- numpy - Numerical computing
- matplotlib & seaborn - Data visualization
- scikit-learn - Machine learning algorithms
  - KMeans (Clustering)
  - PCA (Dimensionality Reduction)
  - Decision Tree & Random Forest (Classification)
  - StandardScaler, LabelEncoder (Preprocessing)
- yellowbrick - Machine learning visualization
- joblib - Model serialization
```

---

## 📁 Struktur File

```
BMLP_Gwyneth_Eunice_Widjaja/
│
├── README.md
│
├── [Clustering]_Submission_Akhir_BMLP_Gwyneth_Eunice_Widjaja.ipynb
│   └── Notebook untuk analisis clustering
│
├── [Klasifikasi]_Submission_Akhir_BMLP_Gwyneth_Eunice_Widjaja.ipynb
│   └── Notebook untuk analisis klasifikasi
│
├── Data/
│   ├── bank_transactions_data_edited.csv
│   ├── bank_transactions_data_edited_.xlsx
│   ├── data_clustering.csv
│   └── data_clustering_inverse.csv
│
└── Models/
    ├── model_clustering.h5
    ├── PCA_model_clustering.h5
    ├── decision_tree_model.h5
    ├── explore_random_forest_classification.h5
    └── tuning_classification.h5
```

---

## 🚀 Cara Menjalankan

### Prerequisites
Pastikan Anda memiliki Python 3.x terinstall di sistem Anda.

### Instalasi Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn yellowbrick joblib
```

### Menjalankan Notebook

1. Clone repository ini:
```bash
git clone https://github.com/[username]/BMLP_Gwyneth_Eunice_Widjaja.git
cd BMLP_Gwyneth_Eunice_Widjaja
```

2. Buka Jupyter Notebook atau Google Colab

3. Jalankan notebook sesuai urutan:
   - Clustering Analysis terlebih dahulu
   - Kemudian Classification Analysis

---

## 📈 Hasil & Insight

### Clustering Analysis
- Berhasil mengelompokkan transaksi ke dalam beberapa cluster
- Menggunakan Silhouette Score untuk evaluasi kualitas clustering
- Visualisasi hasil clustering dengan PCA

### Classification Analysis
- Membandingkan performa berbagai model klasifikasi
- Model terbaik: [Akan diisi setelah evaluasi]
- Akurasi: [Akan diisi setelah evaluasi]

---

## 📝 Catatan

- Dataset diakses langsung melalui Google Sheets untuk memudahkan loading data
- Semua preprocessing dan feature engineering dilakukan sesuai dengan kriteria submission
- Model disimpan dalam format `.h5` menggunakan joblib untuk deployment

---

## 👨‍💻 Pengembang

**Gwyneth Eunice Widjaja**

Submission ini dibuat sebagai bagian dari pembelajaran di platform [Dicoding](https://www.dicoding.com/) - Belajar Machine Learning Pemula.

---

## 📄 Lisensi

Proyek ini dibuat untuk keperluan pembelajaran dan portfolio.

---

## 🙏 Acknowledgments

- Dicoding Indonesia untuk platform pembelajaran yang berkualitas
- Dataset provider untuk data transaksi perbankan
- Komunitas Machine Learning Indonesia

---

**⭐ Jika Anda menemukan proyek ini bermanfaat, jangan lupa untuk memberikan star!**
