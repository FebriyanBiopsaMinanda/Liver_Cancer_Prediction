# 🩺 Liver Cancer Prediction using Machine Learning

## 📌 Deskripsi
Proyek ini berfokus pada **prediksi kanker hati (liver cancer)** berdasarkan data klinis dan gaya hidup pasien.  
Model machine learning diterapkan untuk mengklasifikasikan apakah pasien berisiko atau tidak, berdasarkan kombinasi faktor medis dan kebiasaan hidup.

Algoritma yang digunakan meliputi:
- 🌳 Random Forest  
- 🧩 Support Vector Machine (SVM)  
- 👥 K-Nearest Neighbors (KNN)  
- 📐 Naive Bayes  
- 🌲 Decision Tree  

---

## 📂 Dataset
### 📑 Sumber Data
Dataset diperoleh dari Kaggle:  
🔗 [Predict Liver Cancer – Kaggle](https://www.kaggle.com/datasets/miadul/predict-liver-cancer-from-and-clinical-features/data)

### 📊 Fitur Utama
| Kolom                  | Tipe        | Deskripsi |
|-------------------------|------------|-----------|
| age                    | Numeric    | Usia pasien (30–85 tahun) |
| gender                 | Categorical| Jenis kelamin (Male/Female) |
| bmi                    | Numeric    | Body Mass Index (16–45) |
| alcohol_consumption    | Categorical| Konsumsi alkohol: Never, Occasional, Regular |
| smoking_status         | Categorical| Status merokok: Never, Former, Current |
| hepatitis_b/c          | Categorical| Riwayat infeksi Hepatitis B atau C |
| liver_function_score   | Numeric    | Skor fungsi hati |
| afp_level              | Numeric    | Alpha-fetoprotein (marker kanker hati) |
| family_history         | Categorical| Riwayat kanker hati dalam keluarga |
| cirrhosis              | Categorical| Riwayat sirosis |
| physical_activity      | Numeric    | Aktivitas fisik (jam/minggu) |
| diabetes               | Categorical| Riwayat diabetes |
| liver_cancer           | Target     | Label diagnosis (Yes/No) |

---

## 🔎 Tahapan Analisis
1. **Import Library 📚**  
   Digunakan `pandas`, `numpy`, `matplotlib`, `seaborn`, serta `scikit-learn`.

2. **Load Dataset 📂**  
   Membaca data mentah, eksplorasi awal, dan menampilkan ringkasan variabel.

3. **Data Cleaning 🧹**  
   - Mengecek missing values  
   - Menangani data kosong atau tidak konsisten  

4. **Exploratory Data Analysis (EDA) 📊**  
   - Distribusi pasien berdasarkan usia & gender  
   - Hubungan faktor risiko dengan status kanker hati  
   - Visualisasi korelasi antar variabel numerik  

5. **Preprocessing ⚙️**  
   - Encoding variabel kategorikal  
   - Normalisasi/standarisasi data numerik  
   - Balancing data menggunakan teknik resampling  

6. **Modeling 🤖**  
   Beberapa model diterapkan untuk membandingkan performa:
   - Random Forest  
   - SVM  
   - KNN  
   - Naive Bayes  
   - Decision Tree  

7. **Evaluasi 📈**  
   - Confusion Matrix  
   - Classification Report (Precision, Recall, F1-Score)  
   - Accuracy Score  

---

## 🏆 Hasil

| Model                       | Accuracy  | Precision | Recall  | F1-Score |
|------------------------------|----------|-----------|---------|----------|
| 🌳 Random Forest             | **98.66%** | **0.99** | **0.99** | **0.99** |
| 🧩 Support Vector Machine    | 88.37%   | 0.88      | 0.88    | 0.88     |
| 👥 K-Nearest Neighbors (KNN) | 89.20%   | 0.89      | 0.89    | 0.89     |
| 📐 Naive Bayes               | 83.39%   | 0.83      | 0.83    | 0.83     |
| 🌲 Decision Tree             | 96.10%   | 0.96      | 0.96    | 0.96     |

---

## 📌 Kesimpulan
Berdasarkan hasil evaluasi:  
- 🌳 **Random Forest** memberikan performa **terbaik** dengan akurasi hampir 99% dan skor metrik yang sangat tinggi.  
- 🌲 **Decision Tree** juga cukup baik, namun lebih rentan terhadap overfitting.  
- 🧩 **SVM** dan 👥 **KNN** memiliki performa menengah dengan akurasi ~88–89%.  
- 📐 **Naive Bayes** menjadi model tercepat, tetapi memiliki akurasi paling rendah.

Secara keseluruhan, **Random Forest** adalah model paling optimal untuk prediksi kanker hati pada dataset ini, karena mampu menangkap pola kompleks antar fitur dengan baik.
