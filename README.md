# ⚠️ Important Note
The main Jupyter Notebook (`main_sarima.ipynb`) **exceeds GitHub’s 25 MB upload limit** and cannot be uploaded here.  
You can access the full notebook and model files via Google Drive:

📎 **[View the full notebook and data here](https://drive.google.com/drive/folders/1fmPbjC_zkkp5HK4BP13zebtpUG3HrIMK?usp=drive_link)**

---

# 📈 Forecasting of Indonesian Commodity Prices Using SARIMA

### 🧠 Implementasi Metode Clustering dan Denoising dalam Peramalan Deret Waktu Data Harga Bahan Pangan di Indonesia

This repository contains the research implementation of **Seasonal Autoregressive Integrated Moving Average (SARIMA)** combined with **Clustering** and **Denoising** techniques to forecast Indonesian food commodity prices.  
The project was developed as part of **Arkavidia 9.0 – Datavidia Competition**, representing **Universitas Gadjah Mada (UGM)**.

---

## 🧩 Overview
Fluctuations in food prices are one of the main challenges in maintaining Indonesia’s economic and food stability.  
This project forecasts the prices of **13 key commodities** (e.g., chili, shallots, rice, and cooking oil) by combining:

- 🔹 **Clustering (K-Means)** to group commodities by price volatility  
- 🔹 **Gaussian Wavelet Denoising** to smooth high-volatility data  
- 🔹 **SARIMA Model** to capture seasonal patterns and long-term trends  
- 🔹 **Hyperparameter Tuning** to improve forecasting accuracy  

---

## ⚙️ Methodology
1. **Data Source:** Kaggle *Datavidia 9.0 – Harga Bahan Pangan Dataset* (Jan 2022 – Sep 2024)  
2. **Preprocessing:** Missing value imputation via backward fill, DTW, and linear interpolation  
3. **Feature Extraction:** Coefficient of Variation (CV), MAPC, Rolling Std for volatility grouping  
4. **Modeling:** Comparison between ARIMA and SARIMA  
5. **Evaluation Metric:** Mean Absolute Percentage Error (MAPE)

---

## 📊 Results Summary
| Commodity | Before Tuning (MAPE) | After Tuning (MAPE) | Improvement |
|------------|----------------------|---------------------|--------------|
| Bawang Merah | 45.47 % | 7.01 % | ↓ 38.46 % |
| Cabai Rawit Merah | 14.55 % | 9.35 % | ↓ 5.20 % |
| Cabai Merah Keriting | 18.62 % | 4.91 % | ↓ 13.71 % |

✅ **Average improvement:** 19.1 %  
✅ **SARIMA outperforms ARIMA** in modeling seasonal price fluctuations.

---

## 🧮 Technologies Used
- Python  
- Pandas, NumPy  
- Statsmodels (SARIMA)  
- Scikit-learn (K-Means)  
- PyWavelets (Gaussian Denoising)  
- Matplotlib, Seaborn  

---

## 👨‍💻 Authors
**Krisna Bayu Dharma Putra**, **Nailfaaz**, **Muhammad Dafa Wisnu Galih**  
Department of Computer Science & Electronics – Universitas Gadjah Mada  
📧 dharma.competition@gmail.com  

---

## 🏆 Acknowledgment
This work was created for **Arkavidia 9.0 – Datavidia Competition (2025)**,  
showcasing UGM’s innovation in applying AI and data science for food-price stability.

---

## 📚 Citation
> Putra, K. B. D., Nailfaaz, & Galih, M. D. W. (2025). *Implementasi Metode Clustering dan Denoising dalam Peramalan Deret Waktu Data Harga Bahan Pangan di Indonesia dengan Model SARIMA.* Universitas Gadjah Mada.
