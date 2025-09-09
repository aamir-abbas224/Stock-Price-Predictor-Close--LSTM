# Stock-Price-Predictor-Close--LSTM
This project predicts stock prices using an LSTM neural network built in PyTorch. It trains on Close data ( since the aim was to predict the next Close Price)and forecasts future closing prices based on previous sequences. It works well for most stocks, but highly volatile stocks like NVDA can show steep predicted trends due to rapid price jumps.
