# Transformer-Based Crude Oil Price Forecasting

This project implements a Transformer model to forecast Abu Dhabi Murban crude oil prices based on a 30-day sliding window of historical prices. 
The model evaluates predictive accuracy and simulates hedging actions (BUY / SELL / HOLD) to assess real-world applicability.

## 📁 Files
- `transformer_model.py` — Final transformer code using best hyperparameters.
- `data/2022 AD Murban Crude Oil Futures Historical Data.csv` — Input dataset.
- `requirements.txt` — Required Python libraries.

## 🧠 Model Summary
- Input: 30-day sequences of normalized prices
- Architecture: 2 Transformer blocks + Dense layers
- Optimizer: Adam (0.001)

## 📊 Output
- Predicted vs. actual price plot
- MAE / RMSE
- Hedging decision accuracy table and sample output
