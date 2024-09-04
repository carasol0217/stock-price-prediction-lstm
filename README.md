# README

## Stock Price Prediction using LSTM

This project implements a Long Short-Term Memory (LSTM) neural network to predict NVIDIA (NVDA) stock prices using historical data.

### Overview

The script uses `yfinance` to fetch historical stock prices for NVIDIA from February 17, 2022, to February 17, 2023. It focuses on predicting future prices based on past data.

### Data Fetching

- **Fetch Data:** The `fetch_stock_data` function retrieves daily closing prices using the `yfinance` library.
- **Data Preparation:** Data is scaled and formatted into sequences suitable for training the LSTM model.

### Model Training

- **LSTM Architecture:** The model is composed of three LSTM layers with dropout regularization and a dense output layer.
- **Training:** The model is trained on 80% of the data, with the remaining 20% used for testing. The training involves 50 epochs with a batch size of 32.

### Prediction and Visualization

After training, the model predicts stock prices on the test data, and the results are visualized, comparing the predicted prices to the actual prices.

### Graph:

![Stock Price Prediction](nvidia-prediction.png)


