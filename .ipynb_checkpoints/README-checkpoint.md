# Time Series Forecasting with LSTM on Amazon Stock Prices

This project implements a time series forecasting model using a Long Short-Term Memory (LSTM) neural network in PyTorch. The model is trained on historical Amazon stock prices to predict future prices based on the previous 7-day closing prices.

## Project Overview

The repository provides an end-to-end pipeline for:
- Loading and preprocessing historical stock price data
- Preparing data for LSTM input using a lookback window
- Normalizing the data
- Training an LSTM model
- Visualizing the model’s performance on both training and testing sets.

### Features
- **Data Preprocessing**: Handles date conversion, normalization, and preparation of data for the LSTM network.
- **LSTM Model**: Implements a basic LSTM architecture using PyTorch, with one stacked LSTM layer.
- **Performance Evaluation**: Visualizes both actual and predicted stock prices for the training and testing datasets.
- **GPU Support**: Supports training on GPU using CUDA if available.

## Dataset

The dataset used in this project consists of Amazon stock prices, including the following columns:
- `Date`: The date of the stock price.
- `Close`: The closing price of Amazon's stock on that particular day.

The data is preprocessed to include only the date and closing price.

## Model Architecture

The model is built using the PyTorch framework and consists of the following components:
- **LSTM Layer**: A single LSTM layer with 4 hidden units.
- **Fully Connected Layer**: A linear layer that converts the LSTM output into a single predicted value (stock price).
- **Loss Function**: Mean Squared Error (MSE) to minimize the difference between the predicted and actual stock prices.
- **Optimizer**: Adam optimizer with a learning rate of 0.001.


## Data Preprocessing
## Model Training and Evaluation

During training, the model’s performance is monitored through loss on both the training and validation sets. After training, the predictions for the training and testing sets are visualized.
