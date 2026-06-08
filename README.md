# AOL Scientific Computing — Analisis Produksi Tas EGIER

Tugas akhir mata kuliah Scientific Computing yang menganalisis data produksi tas EGIER (2018–2023) menggunakan empat metode numerik: Polynomial Regression, Taylor Series, Bisection Method, Numerical Differentiation & Integration.

**Nama:** Juan Kevin Utomo  
**NIM:** 2902636856

## Dataset

- **File:** `aol_data.xlsx`
- **Isi:** Data produksi tas biweekly periode Jan 2018 – Dec 2023 (144 titik data)

## Daftar File

| File | Deskripsi |
|------|-----------|
| `Nomor1.ipynb` | Polynomial Regression (Curve Fitting) + Evaluasi R² |
| `Nomor2.ipynb` | Taylor Series Expansion (1–4 suku) |
| `Nomor3.ipynb` | Bisection Method (prediksi waktu konstruksi gudang) |
| `Nomor4.ipynb` | Numerical Differentiation & Integration (Trapezoidal + Simpson) |
| `Soal AoL Scientific Computing.docx` | Soal untuk AoL |
| `AoL_SciComp_Juan Kevin Utomo.pdf` | Laporan akhir format PDF |

## Metode Numerik

| LO | Metode | Deskripsi |
|----|--------|-----------|
| LO1 | Polynomial Regression degree 3 | Least Squares via `np.polyfit`, R² = 0,996 |
| LO3 | Taylor Series | Ekspansi di t = 72, perbandingan 1–4 suku |
| LO2 | Bisection Method | Mencari akar f(t) = P(t) − 25.000 = 0 |
| LO2 | Central Difference | Menghitung laju perubahan produksi |
| LO2 | Trapezoidal & Simpson's 1/3 | Menghitung total produksi |

## Hasil Utama

- **Model:** P(t) = 0,004t³ − 0,134t² + 47,224t + 1748,507 (R² = 0,996)
- **Kapasitas penuh (25.000 tas):** t = 170,374 (Jul 2025)
- **Konstruksi gudang baru mulai:** t = 144,374 (Des 2023)
- **Error integrasi:** Trapezoidal = 0,95%, Simpson's 1/3 = 1,71%

## Referensi

Chapra, S. C., & Canale, R. P. (2015). *Numerical Methods for Engineers* (7th ed.). McGraw-Hill.


