# Stock Market Prediction

## Overview

This repository contains scripts for predicting stock market prices using historical data. It includes tools for training and evaluating a Long Short-Term Memory (LSTM) model for predicting stock prices based on historical data. The project demonstrates how to use machine learning for financial forecasting and can be adapted to various stocks by modifying the parameters.

## Files

- `Google_Stock_Price_Test.csv`: Test dataset containing historical stock prices for Google.
- `Google_Stock_Price_Train.csv`: Training dataset containing historical stock prices for Google.
- `google_stock.py`: Script for training and evaluating an LSTM model using Google stock data.
- `Stock_Market_Prediction.py`: Script for fetching stock data from Yahoo Finance and predicting stock prices for any given stock.

## Usage

### Clone the Repository

```bash
git clone https://github.com/yourusername/stock-market-prediction.git
cd stock-market-prediction
```

## Setup Environment

Ensure you have the required Python packages installed. You can use pip to install them:

```bash
pip install numpy pandas matplotlib scikit-learn keras tensorflow pandas_datareader
```

## Running `google_stock.py`

This script uses historical stock price data to train an LSTM model and predict future stock prices.

### Update File Paths

Modify the file paths in the script to point to the location of `Google_Stock_Price_Train.csv` and `Google_Stock_Price_Test.csv`.

### Run the Script

```bash
python google_stock.py
```

This will train an LSTM model on the Google stock training data and evaluate it on the test data. The script will plot the real vs. predicted stock prices.

## Running `Stock_Market_Prediction.py`

This script fetches stock data from Yahoo Finance and predicts future stock prices.

### Modify Parameters

- Change the `company` variable to the stock ticker symbol you want to predict.
- Adjust the `start` and `end` dates as needed.

### Run the Script

```bash
python Stock_Market_Prediction.py
```

The script will fetch historical stock data, train an LSTM model, and display predictions along with performance metrics.
