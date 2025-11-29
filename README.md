Prediksi Credit Risk Menggunakan Data Pinjaman (2007–2014)

Repository ini berisi project analisis data dan machine learning untuk memprediksi risiko kredit (credit risk) berdasarkan dataset pinjaman dari tahun 2007 hingga 2014.
Proyek ini dilakukan sebagai bagian dari pembelajaran data science dan machine learning, dengan fokus pada pengolahan data, eksplorasi, dan pembuatan model prediksi.

📁 Isi Repository
File	Deskripsi
MAHMUDA_VIX_IDX Partners.ipynb	Notebook utama berisi proses analisis data, pembersihan data, visualisasi, pemodelan, serta evaluasi.
MAHMUDA_VIX_IDX Partners.py	Versi script Python dari proses modeling, cocok untuk dijalankan tanpa notebook.
MAHMUDA_VIX_IDX Partners.pdf	Laporan ringkas hasil analisis dan model prediksi.
📌 Tujuan Proyek

Proyek ini bertujuan untuk:

Mengelompokkan status pinjaman menjadi dua kategori: Aman (1) dan Risiko (0).

Membangun model machine learning untuk memprediksi apakah seorang peminjam berisiko gagal bayar.

Melakukan visualisasi untuk memahami pola dan karakteristik peminjam.

📊 Dataset

Dataset yang digunakan adalah:

loan_data_2007_2014.csv

Jumlah baris: 466.285 data

Jumlah kolom: 75 fitur

Beberapa fitur penting:

loan_amnt, int_rate, dti, annual_inc,

grade, sub_grade, home_ownership, purpose,

dan sebagainya.

🧹 Tahapan Proses Analisis
1. Import Library

Menggunakan berbagai pustaka seperti:

pandas, numpy

matplotlib, seaborn

scikit-learn

SMOTE (imbalance handling)

GridSearchCV

2. Pembersihan & Pemrosesan Data

Langkah-langkah penting:

Menangani missing values dengan SimpleImputer

Menghapus kolom yang tidak relevan

Mengonversi kolom kategorikal

Mengatasi ketidakseimbangan data menggunakan SMOTE

Normalisasi menggunakan StandardScaler

3. Kategorisasi Target (loan_status)

Status pinjaman dikelompokkan menjadi:

🔴 Resiko (0)
Charged Off, Default, Late 31-120 days, In Grace Period, Late 16-30 days,
Does not meet the credit policy. Status: Charged Off

🟢 Aman (1)
Status lain seperti Fully Paid, Current, dll.

📈 Eksplorasi Data (EDA)

Notebook menampilkan beberapa visualisasi, seperti:

Countplot distribusi loan status

Pie chart proporsi aman vs risiko

Boxplot loan_amnt vs loan_status

Scatterplot loan_amnt vs int_rate

Histogram annual_inc

Boxplot dti berdasarkan status

Visualisasi membantu memahami hubungan antara fitur dan status pinjaman.

🤖 Model Machine Learning

Model yang digunakan:

Random Forest Classifier

Menggunakan train-test split

Oversampling memakai SMOTE

Hyperparameter tuning dengan GridSearchCV

Evaluasi model menggunakan:

Accuracy

Precision

Recall

F1-score

ROC-AUC

📌 Hasil Utama

Model Random Forest menunjukkan performa yang baik dalam mendeteksi data kredit berisiko.
Detail skor evaluasi dapat dilihat pada file .ipynb dan laporan .pdf.

🚀 Cara Menjalankan
1. Jalankan Notebook
jupyter notebook MAHMUDA_VIX_IDX Partners.ipynb

2. Jalankan Script Python
python MAHMUDA_VIX_IDX Partners.py

📚 Teknologi yang Digunakan

Python 3.x

Google Colab / Jupyter Notebook

scikit-learn

pandas, numpy

seaborn, matplotlib

✍️ Penulis

Mahmuda
Proyek Data Science — Prediksi Credit Risk
