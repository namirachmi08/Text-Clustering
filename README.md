Text Clustering 

## Identitas Mahasiswa

- **Nama Anggota:**
  
Namira Rachmi Andini (25031554153)

Syahira Nanda Raihanna (25031554199)
- **Program Studi:** S1 Sains Data
- **Fakultas:** Fakultas Matematika dan Ilmu Pengetahuan Alam
- **Universitas:** Universitas Negeri Surabaya
- **Mata Kuliah:** Pemrosesan Teks
- **Dosen Pengampu:** Ulfa Siti Nuraini, S.Stat., M.Stat.
- **Tahun Akademik:** 2026/2027

## Deskripsi Proyek

Proyek ini merupakan pengerjaan Exercise 7 yang membahas penerapan metode clustering dan analisis sentimen pada data teks ulasan film. Dataset yang digunakan berisi ulasan film berbahasa Inggris dengan label sentimen positif dan negatif.

Pengerjaan dilakukan menggunakan Python di Google Colab dengan memanfaatkan beberapa pustaka untuk pengolahan teks, visualisasi, clustering, dan klasifikasi.

## Tahapan Pengerjaan

### 1. Preprocessing Text
Melakukan pembersihan teks yang meliputi:
- Mengubah teks menjadi huruf kecil (*lowercase*).
- Menghapus tag HTML dan URL.
- Menghapus angka dan tanda baca.
- Menghapus spasi berlebih.
- Menghapus *stopwords* bahasa Inggris dengan tetap mempertahankan kata penting seperti `not`, `no`, dan `nor`.

### 2. Feature Engineering
Mengubah teks hasil preprocessing menjadi fitur numerik menggunakan metode **TF-IDF (Term Frequency–Inverse Document Frequency)** agar dapat diproses oleh algoritma machine learning.

### 3. Unsupervised Learning — K-Means Clustering
Menerapkan algoritma K-Means untuk mengelompokkan ulasan berdasarkan kemiripan fitur teks. Percobaan dilakukan dengan jumlah cluster yang berbeda serta menggunakan WordCloud untuk melihat kata-kata dominan pada hasil pengelompokan.

### 4. Unsupervised Learning — Hierarchical Clustering
Menerapkan Agglomerative Clustering untuk membentuk kelompok ulasan berdasarkan kemiripan data. Hasil pengelompokan dianalisis menggunakan jumlah anggota cluster, WordCloud, dan Silhouette Score.

### 5. Sentiment Analysis — WordCloud
Membuat visualisasi WordCloud secara terpisah untuk ulasan dengan sentimen positif dan negatif guna melihat kata-kata yang sering muncul pada masing-masing kelompok.

### 6. Supervised Learning — Random Forest Classification
Melatih model Random Forest menggunakan fitur TF-IDF dan label sentimen untuk memprediksi sentimen ulasan film. Evaluasi dilakukan menggunakan Confusion Matrix dan Classification Report yang mencakup precision, recall, dan F1-score.

### 7. Testing Sentiment
Menguji model menggunakan contoh ulasan baru untuk melihat prediksi sentimen positif dan negatif berdasarkan model yang telah dilatih.

## Tools dan Library

- Python
- Google Colab
- Pandas
- NLTK
- Scikit-learn
- Matplotlib
- WordCloud
- Dataset ulasan film IMDb

## Tujuan

Tujuan pengerjaan ini adalah memahami penerapan preprocessing teks, ekstraksi fitur TF-IDF, metode clustering, visualisasi kata dominan, dan klasifikasi sentimen menggunakan Random Forest.

## Hasil Pengerjaan

Hasil pengerjaan berupa kode program, visualisasi WordCloud, hasil clustering, evaluasi model klasifikasi, dan pengujian prediksi sentimen pada ulasan baru.

