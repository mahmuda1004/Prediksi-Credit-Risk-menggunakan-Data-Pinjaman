# 📊 Prediksi Credit Risk (2007–2014)

Proyek ini berfokus pada analisis data dan pembangunan model machine learning untuk memprediksi **risiko kredit** berdasarkan dataset pinjaman dari tahun **2007 hingga 2014**. Tujuan utama proyek adalah mengklasifikasikan peminjam ke dalam kategori **Aman (1)** atau **Risiko (0)** serta memahami pola yang memengaruhi status pinjaman.

---

## 📁 Isi Repository

- **MAHMUDA_VIX_IDX Partners.ipynb**  
  Notebook utama berisi analisis, pembersihan data, visualisasi, pemodelan, dan evaluasi.

- **MAHMUDA_VIX_IDX Partners.py**  
  Script versi Python dari proses modeling untuk dijalankan di luar notebook.

- **MAHMUDA_VIX_IDX Partners.pdf**  
  Laporan ringkas hasil analisis dan performa model.

---

## 🎯 Tujuan Proyek

- Mengelompokkan status pinjaman menjadi:
  - **1 — Aman**
  - **0 — Risiko**
- Membangun model machine learning untuk memprediksi potensi gagal bayar.
- Melakukan eksplorasi data dan visualisasi untuk memahami karakteristik peminjam.

---

## 📊 Dataset

- **Nama Dataset:** `loan_data_2007_2014.csv`  
- **Jumlah Data:** 466.285 baris  
- **Jumlah Fitur:** 75 kolom  

**Fitur penting yang digunakan:**
`loan_amnt`, `int_rate`, `dti`, `annual_inc`,  
`grade`, `sub_grade`, `home_ownership`, `purpose`, dll.

---

## 🛠️ Tahapan Analisis

### 1. Import Library

Menggunakan library:
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- SMOTE
- GridSearchCV

### 2. Pembersihan & Pemrosesan Data

Proses utama:
- Menangani missing values dengan *SimpleImputer*
- Menghapus kolom yang tidak relevan
- Encoding kolom kategorikal
- Menyeimbangkan data menggunakan **SMOTE**
- Normalisasi fitur menggunakan **StandardScaler**

### 3. Kategorisasi Target (`loan_status`)

**Kategori Risiko (0):**
- Charged Off  
- Default  
- Late 31–120 days  
- Late 16–30 days  
- In Grace Period  
- Does not meet the credit policy: Charged Off  

**Kategori Aman (1):**
- Fully Paid  
- Current  
- Status aman lainnya  

### 4. Eksplorasi Data (EDA)

Visualisasi yang dilakukan:
- Distribusi loan status
- Proporsi aman vs risiko
- Boxplot `loan_amnt` berdasarkan status
- Scatterplot `loan_amnt` vs `int_rate`
- Histogram `annual_inc`
- Boxplot `dti` berdasarkan status

---

## 🤖 Model Machine Learning

**Model utama:** Random Forest Classifier

Penerapan mencakup:
- Train-test split  
- SMOTE untuk mengatasi imbalance data  
- Hyperparameter tuning menggunakan GridSearchCV  

**Metrik yang digunakan:**
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- ROC-AUC  

Detail lengkap performa model tersedia pada file `.ipynb` dan `.pdf`.

---

## 🚀 Cara Menjalankan

### Menjalankan Notebook
```bash
jupyter notebook "MAHMUDA_VIX_IDX Partners.ipynb"
```
## 🔹 Menjalankan Script Python

### Menjalankan Notebook
```bash
python "MAHMUDA_VIX_IDX Partners.py"
```
## Teknologi yang Digunakan
- Python 3.x
- Jupyter Notebook / Google Colab
- scikit-learn
- pandas, numpy
- seaborn, matplotlib

## ✍️ Penulis
### Mahmuda
Proyek Data Science — Prediksi Credit Risk
