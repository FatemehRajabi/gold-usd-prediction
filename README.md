# Gold Price Prediction Using LSTM Neural Network

This project reproduces the "Achilles" paper which predicts the price of Gold vs USD using an LSTM-based deep learning model. It uses technical indicators like moving averages and RSI to improve performance.

## Project Overview

- Predict next-day **gold closing price**
- Data source: Yahoo Finance (`GLD` ETF)
- Model: LSTM neural network with time-series sequences
- Tools: Python, TensorFlow, scikit-learn, pandas, matplotlib

## Notebooks

| File | Description |
|------|-------------|
| `gold_price_lstm_baseline.ipynb` | Initial model using 60-day sequences and 8 features |
| `gold_price_lstm_achilles_reproduction.ipynb` | Refined model using 120-day sequences and additional features like EMA |

## Features Used

- Open, High, Low, Close, Volume
- SMA (10-day, 30-day)
- RSI (14-day)
- EMA (added in refined version)

## Model Results

- Training loss: ~0.0003  
- Validation loss: ~0.0012  
- Predictions follow real prices closely with minor underestimation during sharp rises.

## Requirements

```bash
pip install pandas numpy matplotlib yfinance scikit-learn tensorflow
