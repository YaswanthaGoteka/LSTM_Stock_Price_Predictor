# LSTM_Stock_Price_Predictor
#### This project demonstrates a conceptual PyTorch-based LSTM stock price prediction model using historical market data from Yahoo Finance. The script downloads daily closing prices for a selected stock (default: GOOGL), scales the data, and converts it into fixed-length sequences for time-series learning.

#### A multi-layer LSTM neural network is built from scratch to learn temporal price patterns and predict the next day’s closing price based on the previous 30 days. The model is trained using Mean Squared Error loss and the Adam optimizer, with gradient clipping applied for stability. After training, the model performs inference on the most recent data, inverse-scales the prediction, and generates a simple BUY/SELL signal by comparing the predicted price to the latest real close.

Important Notes:

- **This is not a production-ready trading system—it is a learning-focused, proof-of-concept implementation.**

- GPU usage is expected for proper execution and performance.

 - No backtesting, risk management, or real-world trading constraints are included.

The project is intended to showcase core ideas behind time-series forecasting, LSTM architecture, and PyTorch workflows for financial data analysis.
