# DeltaGroup_JC_DS_FT_Jogja_06_FinalProject

# Optimasi Kampanye Pemasaran Bank: Prediksi Langganan Deposito Berjangka

## Gambaran Proyek
Proyek ini bertujuan untuk mengoptimalkan kampanye telemarketing sebuah bank di Portugal agar lebih banyak nasabah yang berlangganan deposito berjangka. Dataset yang digunakan berasal dari kampanye pemasaran langsung via telepon antara tahun 2008-2010, dengan total **41.188 data** dan **21 fitur**, termasuk data demografi, kontak, riwayat kampanye, dan indikator makroekonomi.

Tantangan utama adalah tingkat konversi yang rendah (~11%) dan biaya kampanye yang tinggi (€0,40 per panggilan, €45 pendapatan per langganan). Dengan model machine learning (XGBoost + SMOTE untuk atasi ketidakseimbangan kelas), proyek ini fokus pada peningkatan targeting dengan target Recall ≥85% dan F2-Score ≥80%.

Lihat dashboard lengkap di [Looker Studio](https://lookerstudio.google.com/u/0/reporting/8bb67993-75b5-4417-bb0e-a285249a94b5/page/p_gf5cymg1td/edit?hl=en).

## Pernyataan Masalah
Kampanye telemarketing bank menghadapi masalah:
- **Tingkat konversi rendah**: Hanya ~11% nasabah yang berlangganan deposito.
- **Biaya peluang tinggi**: Gagal menargetkan nasabah potensial rugi €45, sedangkan salah target hanya rugi €0,40.
- **Penargetan tidak efisien**: Evaluasi data manual bikin boros sumber daya dan ROI rendah.

### Tujuan
1. **Temukan faktor kunci sukses**: Identifikasi minimal 3 fitur penting melalui EDA dan feature importance.
2. **Bangun model prediktif**: Kembangkan model dengan fokus pada Recall untuk penargetan real-time.
3. **Validasi dengan riset eksternal**: Analisis tren makroekonomi dan praktik terbaik telemarketing untuk rekomendasi yang kuat.

## Isi Dataset
Dataset `bank-additional-full.csv` berisi:
- **Jumlah data**: 41.188 baris, 21 kolom.
- **Fitur**:
  - Demografi: `age`, `job`, `education`, `marital`.
  - Kontak: `contact`, `month`, `day_of_week`, `duration` (dihapus untuk hindari data leakage).
  - Riwayat kampanye: `pdays`, `previous`, `poutcome`.
  - Makroekonomi: `emp.var.rate`, `cons.price.idx`, `cons.conf.idx`, `euribor3m`, `nr.employed`.
  - Target: `y` (yes/no untuk langganan deposito).
- **Ketidakseimbangan kelas**: ~11% `y=yes`.

## Prasyarat
Pastikan environment kamu sudah terinstall:
- Python 3.8+
- Library: `pandas`, `numpy`, `scikit-learn`, `imblearn`, `xgboost`, `seaborn`, `matplotlib`, `category_encoders`, `missingno`, `statsmodels`, `lightgbm`.

## Contributor 
Dikembangkan oleh 
- M Rikza N Fachry            [Linkedein](www.linkedin.com/in/mrikzanf)
                              [Github](https://github.com/Rick-zaa)
- Dimas Maulidin Firdaus      [Linkedein](https://www.linkedin.com/in/dhymasmf/)
                              [Github](https://github.com/dhymasmf)
