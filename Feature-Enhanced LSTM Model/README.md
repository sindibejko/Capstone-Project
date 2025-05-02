# Advanced LSTM Model for Crude Oil Price Forecasting

This project implements an advanced LSTM model to forecast Abu Dhabi Murban crude oil prices using technical indicators, external market data, and sentiment signals. 
The model incorporates 8 features across a 10-day rolling window and simulates hedging decisions based on predicted price changes.

## 📁 Files
- `lstm_advanced.py` — Final LSTM model implementation with all features.
- `data/Abu Dhabi Murban Crude Oil Futures Historical Data.csv` — Murban dataset.
- `data/Brent Oil Futures Historical Data.csv` — Brent dataset.
- `data/OVXCLS.csv` — OVX volatility index dataset.
- `requirements.txt` — Required Python libraries.

## 🧠 Model Summary
- Input: 10-day sequences of 8 features:
  - `Price`
  - `Volume`
  - `ATR_14` (Average True Range)
  - `VOL_10` (Rolling volatility)
  - `Brent_Price`
  - `OVX` (Oil Volatility Index)
  - `Sentiment` (from GDELT)
  - `ROC_5` (5-day rate of change)
- Model architecture:
  - LSTM(96 units)
  - Dropout(0.1)
  - Dense(1)
- Optimizer: Adam with learning rate 0.01

## 📊 Output
- Predicted vs. actual price plot
- Residuals plot
- MAE and RMSE scores
- Hedging decision simulation across thresholds (BUY / SELL / HOLD)

## 📌 How to Run

Install dependencies using:

```bash
pip install -r requirements.txt
