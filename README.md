# Stock-Price-Predictor-Close--LSTM
This project predicts stock prices using an LSTM neural network built in PyTorch. It trains on Close data ( since the aim was to predict the next Close Price)and forecasts future closing prices based on previous sequences. It works well for most stocks, but highly volatile stocks like NVDA can show steep predicted trends due to rapid price jumps.TThis project was inspired by a YouTube tutorial and builds on my previous stock predictor. I have improved the code for clarity, ease of use,tested multiple stocks, and customized parts of the workflow myself.
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

**Note:** Highly volatile stocks like **NVDA** may show steep predicted trends due to rapid price jumps, which can cause the model to over-predict sharp rises. This is a result of the stock’s extreme volatility and not a problem with the model itself. See below pictures as examples of the model prediction:

**NVIDIA/NVDA**

<img width="800" height="533" alt="_NVDA" src="https://github.com/user-attachments/assets/1b78a2f0-ae2c-4baa-bd49-3a9ca4e85679" />


**AAPLE/AAPL**

<img width="800" height="533" alt="_AAPL" src="https://github.com/user-attachments/assets/571cb971-86ef-4a15-9e81-e924b276d560" />


**MICROSOT/MSFT**

<img width="800" height="533" alt="_MSFT" src="https://github.com/user-attachments/assets/50756047-c241-4a02-a818-b5db4a2c4da8" />



