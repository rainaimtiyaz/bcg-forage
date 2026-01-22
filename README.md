# PowerCo Customer Churn Analysis
> **BCG X Data Science & Analytics Virtual Experience Program**

## Project Overview
Proyek ini merupakan simulasi konsultasi data science untuk **PowerCo** (perusahaan utilitas energi) di bawah naungan **BCG X**. Fokus utamanya adalah mendeteksi potensi *churn* (perpindahan pelanggan) pada sektor UKM (SME). Melalui analisis data, proyek ini menguji hipotesis apakah sensitivitas harga merupakan pendorong utama *churn* dan memberikan rekomendasi strategi retensi yang efektif.

---

## Key Achievements & Completion
Berdasarkan standar sertifikasi program, berikut adalah poin-poin pencapaian utama dalam proyek ini:

* **Strategic Investigation:** Menyelesaikan simulasi analisis *churn* pelanggan untuk XYZ Analytics dengan mengidentifikasi data klien yang esensial dan menyusun kerangka investigasi strategis.
* **Insightful Data Analysis:** Melakukan analisis data yang efisien menggunakan **Python (Pandas, NumPy)**. Menerapkan teknik visualisasi data untuk interpretasi tren yang mendalam terkait perilaku konsumsi pelanggan.
* **Model Engineering:** Mengembangkan dan mengoptimalkan model **Random Forest** untuk prediksi *churn*. Melalui *feature engineering* yang presisi, model berhasil mencapai **50% Recall Rate** dalam mendeteksi pelanggan yang akan *churn*.
* **Executive Delivery:** Menyusun ringkasan eksekutif (Executive Summary) yang ringkas untuk tim manajemen, memberikan wawasan yang dapat ditindaklanjuti (*actionable insights*) guna mendukung pengambilan keputusan berbasis data.

---

## Data Science Workflow

### 1. Exploratory Data Analysis (EDA)
Menganalisis dataset pelanggan dan harga untuk memahami distribusi *churn*.
* **Key Discovery:** Tingkat *churn* keseluruhan berada di angka ~9.7%.
* **Hypothesis Testing:** Ditemukan bahwa sensitivitas harga memiliki korelasi yang lemah terhadap keputusan pelanggan untuk berhenti, menunjukkan adanya faktor lain (seperti kualitas layanan atau durasi kontrak) yang lebih berpengaruh.

### 2. Feature Engineering
Membangun fitur-fitur baru untuk meningkatkan performa model:
* `offpeak_diff_dec_january_energy`: Mengukur selisih harga dari awal hingga akhir tahun.
* `tenure`: Durasi pelanggan bergabung dengan PowerCo.
* `log_transformation`: Digunakan pada data konsumsi untuk menangani *skewness* dan nilai ekstrem (outlier).

### 3. Predictive Modeling
Menggunakan algoritma **Random Forest Classifier** karena kemampuannya menangani data yang tidak seimbang (*imbalanced data*).
* **Performance:** Akurasi keseluruhan mencapai ~90%.
* **Optimization:** Fokus pada peningkatan *Recall* untuk memastikan sebanyak mungkin pelanggan berisiko tinggi terdeteksi sebelum mereka benar-benar pindah.



---

## Strategic Recommendations
Berdasarkan analisis data dan hasil modeling, rekomendasi strategis bagi PowerCo meliputi:
1.  **Hentikan Diskon Massal:** Karena harga bukan pendorong utama, pemberian diskon ke seluruh pelanggan hanya akan menguras margin tanpa menjamin loyalitas.
2.  **Intervensi Terpilih:** Gunakan model prediktif untuk menargetkan pelanggan dengan skor risiko tinggi dan margin tinggi untuk program retensi khusus.
3.  **Fokus pada Nilai:** Alokasikan anggaran retensi pada akun-akun bernilai tinggi yang diidentifikasi oleh model untuk memaksimalkan ROI.
