# Baseline ARIMA Model for Abu Dhabi Murban Crude Oil Price Forecasting

This file implements a baseline ARIMA(1,1,1) time series model to forecast daily Abu Dhabi Murban crude oil futures prices for the year 2022. 
The model also simulates simple hedging decision strategies based on predicted price changes.

## 📁 Files
- `baseline-arima.py` — Full code including preprocessing, modeling, evaluation, and decision simulation.
- `data/2022 AD Murban Crude Oil Futures Historical Data.csv` — Input dataset (you must upload this to your runtime or clone it into `/content/` if using Colab).
- `requirements.txt` — Required Python libraries.

## 🔍 Main Features
- Loads and cleans raw price data
- Ensures stationarity via differencing and ADF tests
- Fits ARIMA(1,1,1) model using `statsmodels`
- Forecasts prices and evaluates with MAE
- Simulates hedging decisions (BUY / SELL / HOLD) and calculates accuracy

## 📊 Output
- Residual diagnostic plots
- Predicted vs. actual crude oil prices (last 60 business days)
- MAE and RMSE
- Hedging simulation accuracy over multiple thresholds

## 📦 Dependencies
Install dependencies using:

```bash
pip install -r requirements.txt
