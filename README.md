
# Proyek Prediksi Risiko Gagal Bayar Kredit (Credit Default Risk Prediction)

## 1. Ringkasan Eksekutif
Proyek ini membangun model Machine Learning (Random Forest + SMOTE) untuk memprediksi probabilitas Gagal Bayar (*Charged Off*). Model mencapai skor **AUC (Area Under the Curve) sebesar 0.8940**, menunjukkan kekuatan diskriminasi risiko yang sangat baik.

## 2. Hasil Kunci
- **Model:** Random Forest Classifier (dengan SMOTE)
- **Kinerja AUC:** **0.8940**
- **Precision (Charged Off):** 0.92
- **Recall (Charged Off):** 0.48
- **Prediktor Utama:** Suku Bunga (`int_rate`), Kelas Pinjaman (`grade`), dan Jangka Waktu (`term_60 months`).

## 3. Struktur Repositori
Proyek diorganisir sebagai berikut:
- `Notebooks/`: Berisi `Credit_Risk_Analysis_and_Modeling.ipynb` (seluruh alur kerja).
- `Data/processed/`: Berisi `df_final_encoded.csv` (data yang siap untuk ML).
- `Reports/`: Berisi `Laporan_Akhir_Risiko_Kredit.md`.
- `Visualizations/`: Berisi semua plot kunci (Feature Importance, Matriks Kebingungan, dll.).

## 4. Rekomendasi Bisnis
1.  **Tolak Otomatis:** Aplikasi dengan probabilitas risiko di atas ambang batas 50% harus ditolak (didukung oleh Precision 92% model).
2.  **Mitigasi Risiko:** Batasi jangka waktu pinjaman (maksimum 36 bulan) atau terapkan suku bunga premium pada peminjam dengan skor risiko marginal.
