# 📚 Panduan Upload ke GitHub

## Persiapan Awal

### 1. Install Git (jika belum)
Download dan install Git dari: https://git-scm.com/downloads

### 2. Konfigurasi Git (Pertama kali)
Buka Command Prompt atau Git Bash, kemudian jalankan:

```bash
git config --global user.name "Nama Kamu"
git config --global user.email "email@example.com"
```

---

## 🚀 Langkah-langkah Upload ke GitHub

### Opsi 1: Menggunakan Command Line (Recommended)

#### Step 1: Buat Repository Baru di GitHub
1. Login ke GitHub (https://github.com)
2. Klik tombol **"+"** di pojok kanan atas → **"New repository"**
3. Isi detail repository:
   - **Repository name**: `BMLP-Bank-Transaction-Analysis` atau `machine-learning-portfolio`
   - **Description**: "Bank Transaction Analysis using Clustering and Classification - Machine Learning Project"
   - **Public** atau **Private** (pilih sesuai kebutuhan)
   - ❌ **Jangan** centang "Add a README file" (karena sudah ada)
4. Klik **"Create repository"**

#### Step 2: Inisialisasi Git di Folder Lokal
Buka Command Prompt di folder ini, kemudian jalankan:

```bash
# Masuk ke folder proyek
cd "c:\Users\gwyne\Downloads\BMLP_Gwyneth Eunice Widjaja"

# Inisialisasi Git
git init

# Tambahkan semua file ke staging
git add .

# Commit pertama
git commit -m "Initial commit: Bank Transaction Analysis ML Project"
```

#### Step 3: Hubungkan dengan GitHub dan Push

```bash
# Ganti [username] dan [nama-repo] sesuai dengan repository yang kamu buat
git branch -M main
git remote add origin https://github.com/[username]/[nama-repo].git
git push -u origin main
```

**Contoh:**
```bash
git remote add origin https://github.com/gwyneth/BMLP-Bank-Transaction-Analysis.git
git push -u origin main
```

---

### Opsi 2: Menggunakan GitHub Desktop (Lebih Mudah)

#### Step 1: Install GitHub Desktop
Download dari: https://desktop.github.com/

#### Step 2: Login ke GitHub Desktop
Buka aplikasi dan login dengan akun GitHub kamu

#### Step 3: Tambahkan Repository
1. Klik **"File"** → **"Add local repository"**
2. Pilih folder: `c:\Users\gwyne\Downloads\BMLP_Gwyneth Eunice Widjaja`
3. Jika muncul error "not a git repository", klik **"create a repository"**
4. Isi informasi:
   - Name: `BMLP-Bank-Transaction-Analysis`
   - Description: "Bank Transaction Analysis ML Project"
   - Git Ignore: Python
   - License: None atau MIT
5. Klik **"Create Repository"**

#### Step 4: Commit dan Push
1. Lihat semua perubahan di tab "Changes"
2. Tulis commit message: "Initial commit: Bank Transaction Analysis"
3. Klik **"Commit to main"**
4. Klik **"Publish repository"** di bagian atas
5. Pilih **Public** atau **Private**
6. Klik **"Publish Repository"**

---

## 📝 Tips Tambahan

### Membuat Struktur Folder yang Lebih Rapi (Opsional)

Jika ingin mengorganisir file lebih baik, buat struktur seperti ini:

```
BMLP_Gwyneth_Eunice_Widjaja/
│
├── README.md
├── .gitignore
│
├── notebooks/
│   ├── 01_Clustering_Analysis.ipynb
│   └── 02_Classification_Analysis.ipynb
│
├── data/
│   ├── raw/
│   │   ├── bank_transactions_data_edited.csv
│   │   └── bank_transactions_data_edited_.xlsx
│   └── processed/
│       ├── data_clustering.csv
│       └── data_clustering_inverse.csv
│
└── models/
    ├── model_clustering.h5
    ├── PCA_model_clustering.h5
    ├── decision_tree_model.h5
    ├── explore_random_forest_classification.h5
    └── tuning_classification.h5
```

### Update Repository di Masa Depan

Jika ada perubahan file:

```bash
git add .
git commit -m "Update: deskripsi perubahan"
git push
```

### Rename Folder (Opsional)

Jika ingin rename folder menjadi lebih simple:

**Windows:**
```bash
# Di folder Downloads
ren "BMLP_Gwyneth Eunice Widjaja" "BMLP-Bank-Transaction-Analysis"
```

**Nama folder yang disarankan:**
- `BMLP-Bank-Transaction-Analysis`
- `ML-Bank-Transaction-Project`
- `bank-transaction-ml-portfolio`

---

## ⚠️ Troubleshooting

### Error: "remote origin already exists"
```bash
git remote remove origin
git remote add origin https://github.com/[username]/[nama-repo].git
```

### Error: File terlalu besar (>100MB)
GitHub membatasi ukuran file. Jika ada file model yang terlalu besar:
1. Tambahkan ke `.gitignore`
2. Atau gunakan Git LFS: https://git-lfs.github.com/

### Error: Permission denied (publickey)
Gunakan HTTPS URL atau setup SSH key:
https://docs.github.com/en/authentication/connecting-to-github-with-ssh

---

## 🎉 Selesai!

Setelah berhasil upload, repository kamu bisa diakses di:
```
https://github.com/[username]/[nama-repo]
```

Bagikan link ini di CV atau LinkedIn sebagai portfolio! 🚀

---

**Butuh bantuan?** Hubungi:
- GitHub Docs: https://docs.github.com
- Stack Overflow: https://stackoverflow.com
