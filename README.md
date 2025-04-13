# Power-Consumption-Analysis
# AEP Hourly Power Consumption Analysis

This repository contains a time series analysis of hourly power consumption data from AEP (American Electric Power). The project implements data preprocessing, stationarity testing, feature engineering, ARIMA modeling, forecasting, and visualizations, with plans for further enhancements.

## Project Overview

The dataset (`AEP_hourly.csv`) includes:
- **Datetime**: Timestamp of hourly measurements
- **AEP_MW**: Power consumption in megawatts

### Current Features
- **Data Preprocessing**:
  - Convert Datetime, handle duplicates, check for missing values
  - First-order differencing for stationarity
- **Stationarity Testing**:
  - Augmented Dickey-Fuller (ADF) test
  - Kwiatkowski-Phillips-Schmidt-Shin (KPSS) test
- **Feature Engineering**:
  - Extract hour, day of week, month, quarter, and year
- **Modeling**:
  - ARIMA model (p=1, d=1, q=1) for forecasting
- **Evaluation**:
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)
- **Visualizations**:
  - Time series plots (original and differenced) using Plotly
  - ACF and PACF plots for model parameter selection
  - Actual vs. forecasted values

### Planned Enhancements
- Advanced models (e.g., SARIMA, LSTM, Prophet)
- Hyperparameter tuning for ARIMA
- Additional features (e.g., weather data, holidays)
- Cross-validation and extended evaluation metrics
- Interactive dashboards

## Getting Started

### Prerequisites
- Python 3.8+
- Libraries: `pandas`, `numpy`, `matplotlib`, `plotly`, `statsmodels`, `scikit-learn`

Install dependencies:
```bash
pip install -r requirements.txt
