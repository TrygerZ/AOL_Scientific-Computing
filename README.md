# AOL Scientific Computing — Analisis Produksi Tas EGIER

Tugas akhir mata kuliah Scientific Computing yang menganalisis data produksi tas EGIER (2018–2023) menggunakan metode numerik: Polynomial Regression, Model Accuracy Validation, Bisection Method, Numerical Differentiation & Integration.

**Nama:** Juan Kevin Utomo  
**NIM:** 2902636856

## Dataset

- **File:** `aol_data.xlsx`
- **Isi:** Data produksi tas biweekly periode Jan 2018 – Dec 2023 (144 titik data)

## Daftar File

| File | Deskripsi |
|------|-----------|
| `Nomor1.ipynb` | Polynomial Regression degree 3 (Curve Fitting) + plot |
| `Nomor2.ipynb` | Model Accuracy Validation (SSE, MSE, RMSE, MAE, MAPE, R²) |
| `Nomor3.ipynb` | Bisection Method — prediksi waktu konstruksi gudang baru |
| `Nomor4.ipynb` | Numerical Differentiation & Integration (Central Difference, Trapezoidal + Simpson) |
| `Soal AoL Scientific Computing.docx` | Soal untuk AoL |
| `AoL_SciComp_Juan Kevin Utomo.pdf` | Laporan ilmiah format PDF |

## Metode Numerik

| LO | Metode | Deskripsi |
|----|--------|-----------|
| LO1 | Polynomial Regression degree 3 | Least Squares via `np.polyfit`, estimasi tren produksi |
| LO3 | Model Accuracy Validation | SSE, MSE, RMSE, MAE, MAPE, R² = 0,996 |
| LO2 | Bisection Method | Mencari akar f(t) = P(t) − 12.500 = 0 (toleransi 0,001) |
| LO2 | Central Difference | Menghitung laju perubahan produksi (2020 & 2021) |
| LO2 | Trapezoidal & Simpson's 1/3 | Menghitung total produksi kumulatif |

## Hasil Utama

- **Model:** P(t) = 0,004t³ − 0,134t² + 47,224t + 1748,507 (R² = 0,996)
- **SSE:** 11.980.098,288 | **MSE:** 83.195,127 | **RMSE:** 288,436 | **MAE:** 245,304 | **MAPE:** 4,988%
- **Kapasitas penuh (12.500 tas/bi-weekly):** t = 121,865 (Feb 2023)
- **Konstruksi gudang baru mulai:** t = 95,865 (Nov 2021)
- **Bisection konvergen:** 23 iterasi
- **Error integrasi:** Trapezoidal = 0,95%, Simpson's 1/3 = 1,71%
- **Steepest increase 2020:** Nov (624,5 tas/bln) | **2021:** Jul (1.103,5 tas/bln)

## Referensi

Chapra, S. C., & Canale, R. P. (2015). *Numerical Methods for Engineers* (7th ed.). McGraw-Hill.


