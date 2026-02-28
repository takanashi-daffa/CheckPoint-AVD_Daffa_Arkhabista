# CheckPoint-1 Data Gathering & Business Understanding

Nama: Daffa Arkhabista\
NIM: 2509116018

Dataset yang dipakai adalah Brain Stroke Dataset dari Kaggle. Dataset ini berisi data pasien seperti usia, hipertensi, penyakit jantung, kadar gula darah rata-rata, BMI, dan status merokok.

Pada tugas ini, dataset digunakan untuk studi kasus analisis faktor-faktor yang berkaitan dengan risiko stroke. Isi dari file Colab mencakup proses load dataset serta penjelasan Business Understanding seperti tujuan analisis, kondisi dataset, target analisis, dan rencana pengerjaan untuk tahap berikutnya.
---

# CheckPoint-2 Data Understanding & EDA

Pada checkpoint ini dilakukan pemeriksaan kualitas data dan eksplorasi data (EDA) dari Brain Stroke Dataset.

Pemeriksaan meliputi struktur data, statistik deskriptif, tipe data, inconsistent values, missing values, duplicated values, dan outliers. Setelah itu dilakukan EDA menggunakan 4 pilar (Comparison, Composition, Distribution, dan Relationship) untuk melihat pola dan hubungan faktor-faktor terhadap stroke.
---
Dari hasil analisis, usia terlihat memiliki hubungan paling kuat terhadap kejadian stroke, diikuti oleh hipertensi dan penyakit jantung. Dataset dalam kondisi bersih dan siap digunakan untuk tahap berikutnya.
---

# CheckPoint-3 Data Preparation
Pada checkpoint ini dilakukan proses Data Preparation pada Brain Stroke Dataset untuk meningkatkan kualitas data sebelum analisis lanjutan.

### Data Cleaning
Dilakukan pengecekan tipe data, inconsistent values, missing values, duplicated values, dan outliers. Dataset tidak memiliki missing value maupun data duplikat. Penyesuaian tipe data dilakukan pada beberapa kolom kategorikal agar sesuai dengan makna variabel. Outlier dideteksi menggunakan metode IQR dan ditangani dengan membatasi nilai ekstrem pada kolom avg_glucose_level dan bmi tanpa menghapus data.

### Data Construction
Dilakukan pembuatan kolom baru kategori_stroke yang mengubah nilai numerik pada kolom stroke menjadi kategori Stroke dan Tidak Stroke agar data lebih mudah dipahami dan diinterpretasikan.

### Data Reduction
Kolom stroke dihapus karena informasinya sudah direpresentasikan dalam kolom kategori_stroke, sehingga dataset menjadi lebih ringkas dan tidak redundan.
