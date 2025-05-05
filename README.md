
# 📊 Analisis Sentimen Media Sosial

Proyek ini bertujuan untuk menganalisis sentimen dari konten yang dihasilkan pengguna di berbagai platform media sosial seperti Twitter, Instagram, dan Facebook. Dengan menggunakan teknik pemrosesan bahasa alami (NLP) dan algoritma pembelajaran mesin, proyek ini mengklasifikasikan sentimen dari setiap postingan menjadi positif, negatif, atau netral.

## 📁 Dataset

Dataset yang digunakan adalah [Social Media Sentiments Analysis Dataset](https://www.kaggle.com/datasets/kashishparmar02/social-media-sentiments-analysis-dataset) yang disediakan oleh Kashish Parmar di Kaggle. Dataset ini berisi 733 entri dengan 15 kolom yang mencakup informasi seperti teks postingan, sentimen, waktu, platform, hashtag, jumlah retweet dan like, serta informasi geografis.

### Struktur Dataset

- `Unnamed: 0`: Indeks (dapat diabaikan)
- `Text`: Konten teks dari postingan pengguna
- `Sentiment`: Label sentimen (Positive, Negative, Neutral)
- `Timestamp`: Tanggal dan waktu postingan
- `User`: Nama pengguna yang memposting
- `Platform`: Platform media sosial (Instagram, Facebook, Twitter, dll.)
- `Hashtags`: Hashtag yang digunakan dalam postingan
- `Retweets`: Jumlah retweet
- `Likes`: Jumlah like
- `Country`: Negara asal postingan
- `Year`, `Month`, `Day`, `Hour`: Komponen waktu yang diekstrak dari timestamp

## 🎯 Tujuan Proyek

- Melakukan praproses data teks untuk analisis sentimen
- Membangun model klasifikasi untuk mengkategorikan sentimen
- Mengevaluasi performa model menggunakan metrik seperti akurasi, presisi, recall, dan F1-score
- Menganalisis tren sentimen berdasarkan waktu, platform, dan lokasi geografis

## 🛠️ Cara Penggunaan

1. **Klon repositori ini:**

   ```bash
   git clone https://github.com/username/analisis-sentimen-media-sosial.git
   cd analisis-sentimen-media-sosial
   ```

2. **Instal dependensi:**

   Pastikan Anda memiliki Python 3.x dan pip terinstal. Kemudian instal dependensi yang diperlukan:

   ```bash
   pip install -r requirements.txt
   ```

3. **Unduh dataset:**

   Unduh dataset dari [Kaggle](https://www.kaggle.com/datasets/kashishparmar02/social-media-sentiments-analysis-dataset) dan tempatkan file `sentimentsdataset.csv` di direktori proyek.

4. **Jalankan notebook:**

   Buka dan jalankan notebook Jupyter `SentimentAnalysis.ipynb` untuk melihat proses analisis dan hasilnya.

## 📊 Hasil Model

Beberapa algoritma pembelajaran mesin telah diterapkan dan dievaluasi. Berikut adalah ringkasan performa model:

| Model                 | Akurasi  | Presisi | Recall  | F1-Score |
|-----------------------|----------|---------|---------|----------|
| Random Forest         | 77.55%   | 68.28%  | 77.55%  | 69.84%   |
| Extra Trees           | 79.59%   | 70.02%  | 79.59%  | 74.20%   |
| K-Nearest Neighbors   | 76.87%   | 71.99%  | 76.87%  | 74.08%   |
| Decision Tree         | 76.87%   | 75.53%  | 76.87%  | 75.21%   |
| Logistic Regression   | 76.19%   | 58.05%  | 76.19%  | 65.89%   |
| Naive Bayes           | 76.19%   | 58.05%  | 76.19%  | 65.89%   |
| AdaBoost              | 76.19%   | 58.66%  | 76.19%  | 66.27%   |
| SVM                   | 76.87%   | 60.09%  | 76.87%  | 67.43%   |
| Gradient Boosting     | 74.15%   | 67.48%  | 74.15%  | 70.47%   |

Model **Extra Trees** menunjukkan performa terbaik dengan akurasi 79.59% dan F1-score 74.20%.

## 📈 Visualisasi

Analisis visual dilakukan untuk memahami distribusi sentimen, aktivitas berdasarkan platform, dan tren temporal. Beberapa temuan utama:

- **Distribusi Sentimen:** Sentimen positif mendominasi, diikuti oleh netral dan negatif.
- **Aktivitas Platform:** Twitter memiliki jumlah postingan terbanyak, namun Instagram menunjukkan tingkat interaksi (likes dan retweets) yang lebih tinggi.
- **Tren Temporal:** Aktivitas postingan meningkat pada jam-jam tertentu, menunjukkan pola penggunaan media sosial yang konsisten.

## 📄 Lisensi

Dataset ini berada dalam domain publik (CC0: Public Domain). Proyek ini menggunakan lisensi MIT. Silakan merujuk ke file [LICENSE](LICENSE) untuk informasi lebih lanjut.

## 🙏 Kontribusi

Kontribusi sangat diterima! Jika Anda memiliki saran, perbaikan, atau ingin menambahkan fitur baru, silakan buat pull request atau buka issue.

---
