# LSTM Stock Price Prediction (PyTorch)

## Overview
This project implements a PyTorch-based LSTM model to predict stock closing prices using historical data from Yahoo Finance. Given the past 30 days of price data, the model learns temporal patterns and forecasts the next day’s closing price.

The pipeline includes data preprocessing, sequence generation, model training, and inference, ending with a simple BUY/SELL signal based on predicted vs actual prices.

## Features
- Time-series forecasting using LSTM neural networks
- Automated data collection via Yahoo Finance
- Data normalization and sequence generation
- Multi-layer LSTM architecture built from scratch
- Gradient clipping for training stability
- Inference pipeline with inverse scaling
- Basic trading signal generation (BUY/SELL)

## Model Details
- Input: 30-day sliding window of closing prices
- Architecture: Multi-layer LSTM + Fully Connected layer
- Loss Function: Mean Squared Error (MSE)
- Optimizer: Adam
- Output: Next-day predicted closing price

## Example Workflow
1. Download historical stock data (default: GOOGL)
2. Normalize and convert data into sequences
3. Train LSTM model on time-series data
4. Predict next-day price
5. Generate BUY/SELL signal

## Limitations
- Not a production-ready trading system
- No backtesting or evaluation on unseen market regimes
- No risk management or transaction cost modeling
- Uses only closing price (limited feature set)

## Future Improvements
- Implement advanced architectures (GRU, Transformers)
- Add technical indicators, volume, and macroeconomic features
- Perform walk-forward validation for realistic evaluation
- Hyperparameter optimization (Grid Search / Bayesian methods)
- Integrate backtesting framework

## Tech Stack
- Python
- PyTorch
- NumPy / Pandas
- yFinance
- Scikit-learn

## Disclaimer
This project is for educational purposes only and should not be used for real trading decisions.
