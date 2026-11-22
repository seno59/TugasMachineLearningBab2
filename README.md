# TugasMachineLearning
# Laporan Praktikum Machine Learning: Diagnosis Bias-Variance & CRISP-DM

## Praktikum 1: Pemetaan Proyek Nyata ke CRISP-DM (Telco Customer Churn)
1. *Business Understanding:* Menetapkan tujuan memprediksi pelanggan yang berpotensi churn untuk menekan churn rate perusahaan.
2. *Data Understanding:* Mengumpulkan dan mengidentifikasi fitur pelanggan (durasi langganan, metode pembayaran, total tagihan).
3. *Data Preparation:* Penanganan missing value, manipulasi tipe data, one-hot encoding, dan penskalaan fitur.
4. *Modeling:* Melatih model klasifikasi (Decision Tree Classifier) dengan berbagai variasi kedalaman (max_depth).
5. *Evaluation:* Mengukur performa model dengan metrik evaluasi dan menganalisis grafik learning curve.
6. *Deployment:* Mengintegrasikan model terbaik ke sistem operasional untuk early warning tim Customer Retention.

---

## Praktikum 2: Diagnosis Bias-Variance (Decision Tree)

### Hasil Perhitungan/Output Kode:
- *max_depth = 1:* Underfitting (High Bias)  
  Alasan: Skor train dan validasi sama-sama rendah dengan gap yang kecil karena model terlalu sederhana (stump).
- *max_depth = 4:* Seimbang / Good Fit (Optimal Bias-Variance)  
  Alasan: Skor train dan validasi keduanya berada pada tingkat yang tinggi dengan gap yang minimal.
- *max_depth = None:* Overfitting (High Variance)  
  Alasan: Skor train sangat tinggi (mendekati 1.000), namun skor validasi turun drastis (gap antara train dan validasi sangat besar) karena pohon tumbuh tanpa batas.
