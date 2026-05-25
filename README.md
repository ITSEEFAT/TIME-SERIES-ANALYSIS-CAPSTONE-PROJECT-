# Time Series Analysis & Portfolio Forecasting (TSA 2026)

A deep learning-based financial time series forecasting project focused on predicting short-term stock prices using multiple neural network architectures and evaluating their real-world portfolio performance.

## Live Demo
https://tsa2026-portfolio-dashboard.netlify.app/

---

## Project Overview

This project explores the application of Deep Learning models for stock price forecasting on Indian equities.

The workflow includes:

- Historical stock data collection from Yahoo Finance
- Data preprocessing and scaling
- Sequence generation using rolling windows
- Training multiple DL models:
  - LSTM
  - GRU
  - CNN
  - Transformer
- Performance comparison using regression metrics
- Live prediction on unseen trading days
- Portfolio construction using inverse volatility allocation
- Interactive dashboard deployment

---

## Models Used

### 1. LSTM (Long Short-Term Memory)
Captures long-term temporal dependencies in stock price sequences.

### 2. GRU (Gated Recurrent Unit)
Computationally efficient alternative to LSTM.

### 3. CNN (1D Convolutional Neural Network)
Extracts local temporal patterns from price windows.

### 4. Transformer
Attention-based architecture for sequence modeling.

---

## Key Results

### Historical Test Performance
- LSTM/GRU hybrid consistently outperformed CNN and Transformer
- Lower MAPE and RMSE across most stocks

### Live Trading Performance
Forecasts were tested on a 2-day live trading window.

| Stock | Direction Correct | Live MAPE |
|------|------|------|
| DIXON.NS | Yes | 10.86% |
| DEEPAKNTR.NS | Yes | 3.89% |
| ASTRAL.NS | No | 10.61% |
| COFORGE.NS | Yes | 32.00% |
| PERSISTENT.NS | Yes | 33.04% |
| ABB.NS | No | 18.08% |
| APOLLOHOSP.NS | No | 12.03% |

**Best Live MAPE:** DEEPAKNTR.NS → 3.89%  
**Directional Accuracy:** 4/7 stocks

---

## Portfolio Strategy

Implemented **Inverse Volatility Portfolio Allocation**:

- Lower volatility stocks receive higher capital allocation
- Risk-balanced portfolio construction

Portfolio evaluated on:
- Day 1 predicted allocation
- Day 2 predicted allocation
- Actual vs predicted returns

---

## Tech Stack

- Python
- TensorFlow / Keras
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- yFinance
- HTML/CSS/JavaScript
- Netlify


---

## Features

- Multi-model stock forecasting
- Live 2-day forecasting
- Portfolio optimization
- Interactive deployed dashboard
- Performance visualizations
- Real-world evaluation pipeline

---

## Dashboard Preview

Visit:
https://tsa2026-portfolio-dashboard.netlify.app/

---

## Future Improvements

- Add technical indicators (RSI, MACD, Bollinger Bands)
- Sentiment analysis from financial news
- Walk-forward validation
- Ensemble forecasting
- Temporal Fusion Transformers
- Larger dataset coverage

---

## Report

Detailed project report included in repository.

Covers:
- Methodology
- Model comparison
- Portfolio logic
- Results
- Reflections and future work

---

## Author

**SYED SEEFATUL HAQUE**  
GLBITM

GitHub: https://github.com/ITSEEFAT
