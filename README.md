<img width="1182" height="788" alt="image" src="https://github.com/user-attachments/assets/ff4bcd79-6933-4c33-939a-fe21d071323c" /># Stock-Price-Predictor-Close--LSTM
This project predicts stock prices using an LSTM neural network built in PyTorch. It trains on Close data ( since the aim was to predict the next Close Price)and forecasts future closing prices based on previous sequences. It works well for most stocks, but highly volatile stocks like NVDA can show steep predicted trends due to rapid price jumps.

Features:
  Uses historical stock data from Yahoo Finance
  LSTM implemented in PyTorch
  Normalizes data using StandardScaler
  Predicts future closing prices from past sequences
  Visualizes actual vs predicted prices and prediction error

Choose a stock:
  Change the ticker symbol in the script (default: NVDA)
  The model will train and display predicted vs actual prices  

How it Works:
  Download historical stock data using yfinance.
  Normalize closing prices using StandardScaler.
  Create sequences of length seq_length for LSTM input.
  Train an LSTM model to predict the next closing price.
  Evaluate predictions using RMSE and visualize results.  

**Note:** Highly volatile stocks like **NVDA** may show steep predicted trends due to rapid price jumps, which can cause the model to over-predict sharp rises. This is a result of the stock’s extreme volatility and not a problem with the model itself.
