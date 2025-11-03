
# LAPORAN AKHIR PROYEK DATA SCIENCE: MODEL PREDIKSI RISIKO KREDIT
## 1. Ringkasan Eksekutif
Proyek membangun model Random Forest + SMOTE dengan AUC 0.8940. Model sangat baik dalam diskriminasi risiko.
## 2. Metodologi
- Model: Random Forest Classifier
- Penanganan Imbalance: SMOTE
## 3. Temuan Utama (Feature Importance)
Pendorong risiko terkuat: Suku Bunga (`int_rate`), Kelas Pinjaman (`grade`), dan Jangka Waktu (`term`).
## 4. Kinerja Model
- AUC Score: 0.8940 (Sangat Baik)
- Precision (Charged Off): 0.92 (Tinggi)
- Recall (Charged Off): 0.48 (Moderat)
## 5. Rekomendasi Bisnis
1. Tolak Otomatis: Aplikasi dengan risiko > 50% (berdasarkan Precision 92%).
2. Mitigasi: Batasi jangka waktu pinjaman untuk peminjam berisiko marginal.
