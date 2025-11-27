# Heatwave_Forecast_Prediction_IMD
Delhi Heatwave Forecasting using Machine Learning (1970–2024) A complete end-to-end AI/ML project developed during my internship at the Indian Meteorological Department (IMD). Includes station-wise data preprocessing, feature engineering, heatwave labeling using IMD criteria, Random Forest modeling, and forecast evaluation on 2024 data.

# Overview

This project focuses on heatwave prediction and forecasting for Delhi using over 50 years of station-wise meteorological data (1970–2024) obtained from the Indian Meteorological Department (IMD).
It was completed as part of my 6-week IMD internship (extended to 7 weeks).

The project covers:
1) Data preprocessing of long-term station-wise data
2) Feature engineering and climatology-based heatwave labeling
3) Nowcasting models using Random Forest
4) Forecasting models using lag features
5) Evaluation on unseen year 2024
6) Station-wise comparative performance

# Stations Used
The following IMD stations were used:
1) Ayanagar
2) Safdarjung
3) Palam

# Project Objectives

- Build a machine learning system capable of predicting heatwave intensity and temperature anomalies.
- Develop forecasting models using lag-based features (1–7 day lags).
- Generate IMD-standard heatwave labels using 30-year climatology (1993–2023).
- Compare nowcast vs. forecast performance for multiple stations.

# Tech Stack
- Python, Google Colab
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Pickle (model saving)
- Random Forest Regressor (main algorithm)
- Google Drive integration

# Heatwave Labeling Criteria (IMD Standard)

Heatwave = max_temp – normal_temp > 4.5°C, OR
normal_temp ≥ 40°C

Normal temperature was computed using 30-year climatology (1993–2023).

# Machine Learning Models
1️⃣ Nowcast Models (Same-Day Prediction)
   - Random Forest Regressor
   - Trained on cleaned dataset
Features included max temp, min temp, humidity, DBT, RH, etc.

2️⃣ Forecast Models (Next-Day Prediction)
   - Lag-based features (1–7 day lag)
     Train: 1970–2023
     Test: Only 2024

Evaluated real forecasting accuracy!

