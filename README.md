# Indoor Air Quality Prediction Using Machine Learning

## Overview
This project applies machine learning models to analyze and predict indoor air quality using real-world environmental sensor data collected in Italy.

Two tasks are addressed:
- Regression: Predicting carbon monoxide concentration (CO_GT)
- Classification: Categorizing air quality levels into Low, Medium, and High

## Dataset
- AirQualityUCI dataset (hourly indoor sensor readings)
- Features include gas concentrations (CO, NO2, NMHC, C6H6), temperature, humidity, and absolute humidity

## Data Preparation
- Replaced missing value markers (-200) with NaN
- Dropped incomplete and irrelevant columns
- Created custom air quality labels (CO_Quality_Level)

## Models
- Random Forest Regressor – for predicting CO_GT
- Random Forest Classifier – for classifying air quality levels

## Evaluation
**Regression:**
- RMSE ≈ 34.7
- R² ≈ 0.80

**Classification:**
- Accuracy ≈ 86%
- F1-scores ≈ 0.86–0.87 across classes

## Insights
Key pollutant features (NOx_GT, C6H6_GT, NMHC_GT) were identified as the strongest indicators of air quality.

## Tools
Python, Pandas, NumPy, Matplotlib, scikit-learn

## How to Run
Open `project1ML.ipynb` in Google Colab or Jupyter Notebook and run all cells.

