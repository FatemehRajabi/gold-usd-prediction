# Gold Price Prediction Using LSTM Neural Network: A Reproduction Study

This project reproduces parts of the paper "Achilles, Neural Network to Predict the Gold Vs US Dollar Integration with Trading Bot for Automatic Trading" by Angel Varela. The goal is to forecast the next-day closing price of gold (XAUUSD) using an LSTM-based deep learning model, enhanced with technical indicators like moving averages and RSI.

## Project Overview

- Prediction Target: Next-day gold closing price
- Data Source: Yahoo Finance (GLD ETF)
- Model: LSTM neural network using a 60-day sequence window
- Tools: Python, TensorFlow, scikit-learn, pandas, matplotlib

## Notebooks

| File | Description |
|------|-------------|
| `Baseline_Model_ARIMA.ipynb` | ARIMA baseline model for gold price forecasting |
| `Main_Model_LSTM.ipynb` | Main LSTM model using 60-day sequences with technical indicators |

## Features Used

- Price Features: Open, High, Low, Close, Volume
- Technical Indicators:
- SMA (Simple Moving Average) — 10-day and 30-day
- RSI (Relative Strength Index) — 14-day

## Model Results

- ARIMA Performance:
    RMSE: 16.69
    MAE: 13.91

- LSTM Performance:
    RMSE: 4.37
    MAE: 3.54

- Observations:
    The LSTM model closely tracks the real gold price, capturing both trends and short-term fluctuations better than ARIMA.

## Requirements

```bash
pip install pandas numpy matplotlib yfinance scikit-learn tensorflow
