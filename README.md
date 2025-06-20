
# 🧠 Sentiment Analysis with TF-IDF, SVM, and Random Forest

Proyek ini melakukan analisis sentimen terhadap data ulasan menggunakan pendekatan machine learning klasik. Model yang digunakan adalah **SVM** dan **Random Forest**, dikombinasikan dengan teknik ekstraksi fitur seperti **TF-IDF**, **Chi-Square**, dan penyeimbangan data **SMOTE**.

---

## 📂 Dataset

- Dataset: `bsi_reviews.csv`
- Kolom:
  - `content` — Teks ulasan
  - `polarity` — Label sentimen (positif, negatif, netral)

---

## ⚙️ Arsitektur Model

### ✅ Skema 1: Random Forest + TF-IDF + Cross Validation (5-Fold)
- Teknik: TF-IDF (min_df=5, max_df=0.85)
- Evaluasi: 5-Fold Cross Validation
- Rata-rata Akurasi: **84.34%**

### ✅ Skema 2: Random Forest + TF-IDF + Chi-Square + SMOTE
- Teknik: TF-IDF + Chi-Square + SMOTE
- Split: 90% training / 10% testing
- Akurasi Test: **90.86%**

### ✅ Skema 3: SVM + TF-IDF + SMOTE
- Teknik: TF-IDF + SMOTE
- Split: 90% training / 10% testing
- Akurasi Test: **88.83%**

---

## 🛠️ Instalasi

1. Clone repositori ini:
   ```bash
   git clone https://github.com/username/sentiment-analysis-tfidf.git
   cd sentiment-analysis-tfidf
   ```

2. Buat virtual environment (opsional tapi disarankan):
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/macOS
   venv\Scripts\activate   # Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## 📊 Hasil Evaluasi

| Skema   | Model | Teknik Tambahan        | Akurasi Test |
|---------|--------|------------------------|--------------|
| Skema 1 | RF     | TF-IDF + 5-Fold CV     | 84.34%       |
| Skema 2 | RF     | TF-IDF + Chi2 + SMOTE  | **90.86%**   |
| Skema 3 | SVM    | TF-IDF + SMOTE         | 88.83%       |

---

## 📌 Rencana Pengembangan

- [ ] Tuning hyperparameter (GridSearchCV)
- [ ] Eksperimen dengan n-gram TF-IDF
- [ ] Uji model deep learning (LSTM/CNN)
- [ ] Visualisasi confusion matrix dan akurasi

---

## 👨‍💻 Author

- Nama: *[Isi Nama Anda]*
- Email: *[Isi Kontak Anda]*
- Dibuat dengan ❤️ untuk analisis teks bahasa Indonesia

---

## 📄 License

Proyek ini dilisensikan di bawah MIT License. Lihat file [LICENSE](LICENSE) untuk detail.
