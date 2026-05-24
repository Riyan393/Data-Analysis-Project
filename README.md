# Blockchain Cryptocurrency Price Forecasting with Machine Learning

> MSc Dissertation — IT with Data Analytics | University of the West of Scotland | 2026

## Overview

This project investigates the application of machine learning algorithms to forecast cryptocurrency price movements (Bitcoin & Ethereum) using historical price data and technical indicators. Twelve ML and deep learning models were benchmarked against each other using R², MAE, and RMSE as evaluation metrics.

**Key finding:** Bayesian Ridge achieved the highest predictive accuracy overall, while deep learning models (1D CNN, GRU) better captured non-linear temporal patterns in highly volatile periods.

---

## Models Evaluated

| Category | Models |
|---|---|
| Classical ML | Bayesian Ridge, Linear Regression, K-Nearest Neighbors (KNN), Decision Tree |
| Ensemble | Random Forest, Gradient Boosting, AdaBoost |
| Support Vector | Support Vector Regressor (SVR) |
| Deep Learning | LSTM, GRU, Simple RNN, 1D Convolutional Neural Network (CNN) |

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-green?logo=scikit-learn)
![TensorFlow](https://img.shields.io/badge/TensorFlow-DeepLearning-orange?logo=tensorflow)
![Pandas](https://img.shields.io/badge/Pandas-DataProcessing-blue?logo=pandas)

**Languages & Libraries:** Python, Pandas, NumPy, Scikit-learn, TensorFlow/Keras, Matplotlib, Seaborn

---

## Methodology

1. **Data Collection** — Historical OHLCV data for Bitcoin and Ethereum
2. **Preprocessing** — Missing value handling, normalisation, feature engineering (moving averages, RSI, Bollinger Bands, MACD)
3. **Data Splitting** — Train/test split with time-series integrity preserved
4. **Model Training** — 12 models trained across classical ML, ensemble, and deep learning families
5. **Evaluation** — Models ranked by R² Score, MAE, and RMSE
6. **Results Analysis** — Performance comparison with visualisations across all model groups

---

## Results Summary

| Model Group | Top Performer | Metric Strength |
|---|---|---|
| Group 1: Bayesian Ridge, KNN, 1D CNN | **Bayesian Ridge** | Best R², lowest MAE & RMSE |
| Group 2: GRU, SVR, Gradient Boosting | **Gradient Boosting** | Strong R², consistent MAE |
| Group 3: Simple RNN, AdaBoost, Decision Tree | **AdaBoost** | Best generalisation |
| Group 4: Linear Regression, Random Forest, LSTM | **LSTM** | Best temporal pattern capture |

**Overall winner: Bayesian Ridge** — highest predictive accuracy across all three evaluation metrics.

Deep learning models (1D CNN, GRU) demonstrated superior ability to capture non-linear and temporal relationships, suggesting hybrid approaches may yield further improvements.

---

## Key Findings

- Bayesian Ridge outperformed all deep learning models on standard metrics due to regularisation properties on noisy financial data
- Ensemble methods (Gradient Boosting, Random Forest) offered strong generalisation across volatile periods
- Deep learning models (LSTM, GRU) showed greater potential for long-term temporal dependency modelling
- Feature engineering (technical indicators) significantly improved model performance over raw price data alone
- Future work: incorporate real-time sentiment data (Twitter/Reddit NLP) and macroeconomic indicators

---

## Project Structure

```
├── data/                  # Raw and processed datasets
├── notebooks/             # Jupyter notebooks for each model group
├── models/                # Saved model files
├── results/               # Performance metrics and visualisations
└── README.md
```

---

## Author

**Riyan Ahmed Baig**  
MSc IT with Data Analytics — University of the West of Scotland  
[LinkedIn](https://www.linkedin.com/in/riyan393) · [GitHub](https://github.com/Riyan393)

---

*Completed as part of the MSc dissertation requirements at the University of the West of Scotland (2026).*
