# Bayesian-Machine-Learning
This repository contains projects that apply Bayesian methods for financial time series forecasting and model optimization. The goal is to improve prediction accuracy and capture uncertainty using Bayesian approaches.

# Projects

# 1. Bayesian Optimization for Forex Prediction

  Applied Bayesian optimization with skopt (BayesSearchCV) to tune LightGBM, CatBoost, and XGBoost models.
  Dataset: EUR/USD hourly Bid Close prices.
  Train: pre-2020, Test: 2020 (COVID period).

**Workflow**:

    Data preprocessing & feature engineering.
    Hyperparameter tuning with Bayesian optimization.
    Evaluation using RMSE, MAE.
    Visual comparison of Actual vs Predicted prices.

**Results**:

  Bayesian optimization improved prediction performance compared to default parameters.
  LightGBM and CatBoost tracked 2020 volatility effectively.

# 2. Bayesian ARIMA Forecasting

Applied Bayesian ARIMA for monthly stock price forecasting.
Dataset: MARI_KA_Monthly.csv (Adj_Close prices).

**Workflow**:

  Differenced series for stationarity.
  Priors defined for AR (phi), MA (theta), and error terms.
  Monte Carlo simulations for posterior sampling.
  Forecasted 12 months ahead with uncertainty bands.

# Results:

Provided prediction intervals instead of single point forecasts.
Captured uncertainty in financial time series effectively.
