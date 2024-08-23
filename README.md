Overview
This project aims to forecast the future prices of Ethereum (ETH) using the Temporal Fusion Transformer (TFT) model implemented in PyTorch Lightning. The project leverages historical data from the CryptoCompare API to predict the next 7 days' closing prices of ETH/USD. The prediction is based on 2000 days of historical price data, making it suitable for analyzing and forecasting trends in highly volatile markets like cryptocurrencies.

Project Structure
Data Fetching: The code fetches historical daily price data for Ethereum using the CryptoCompare API. The data includes time, open, high, low, close prices, and trading volume.

Data Preprocessing: The dataset is preprocessed and transformed into a format suitable for time series forecasting, including features such as time indices, group identifiers, and scaling.

Model: The Temporal Fusion Transformer model is employed for the forecasting task. It is designed to handle various features, including time-varying known and unknown reals, and is optimized with QuantileLoss to predict a range of possible future prices.

Training: The model is trained using PyTorch Lightning, with support for GPU acceleration. Early stopping and learning rate monitoring are implemented to enhance the training process.

Prediction: After training, the model predicts the next 7 days' prices, which are then plotted and compared to historical data for visualization.

![download](https://github.com/user-attachments/assets/90095052-7e21-41b6-a1bb-41958fbce3b7)


