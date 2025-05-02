# Baseline LSTM Model for Abu Dhabi Murban Crude Oil Price Forecasting

This project implements a baseline LSTM model to forecast Murban crude oil futures prices using historical data. It uses a sequence of past 10 days (price and volume) to predict the next day's price, and includes a hedging decision simulation based on model predictions.

## 📁 Files
- `lstm_baseline_final.py` — Clean final version of the LSTM model (no tuning logic).
- `data/2022 AD Murban Crude Oil Futures Historical Data.csv` — Input dataset (to be uploaded if using Colab).
- `requirements.txt` — Required Python libraries.

## 🧠 Model Summary
- Input features: Scaled Price & Volume
- Sequence length: 10 days
- Model architecture:
  - LSTM(96 units)
  - Dropout(0.1)
  - Dense(1)
- Optimizer: Adam with learning rate 0.01

## 📊 Output
- Plots comparing actual vs. predicted crude oil prices.
- Residual error plot.
- Evaluation metrics: MAE & RMSE.
- Hedging decision simulation over multiple thresholds (BUY / SELL / HOLD).

## 💻 How to Run
1. Upload the `.csv` file.
2. Install dependencies.
3. Run the script.

To install dependencies:
```bash
pip install -r requirements.txt
