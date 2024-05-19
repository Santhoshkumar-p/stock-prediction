# Stock Price Prediction using LSTM Networks
GME Stock Prediction with historical data and sentiment analysis

## Abstract:
This project developed LSTM models to predict stock prices using historical data. LSTM networks are well-suited for time-series forecasting tasks. Daily stock price data for GameStop (GME) for 2021 was used. LSTM models with 1 or 2 hidden layers were trained to predict next-day closing prices based on previous 10 days prices. The models achieved low error on test data, demonstrating the feasibility of using LSTM networks for stock prediction.

## Introduction:
- Stock price prediction is crucial for financial forecasting. Traditional models like ARIMA have limitations in capturing nonlinear patterns. LSTM networks are adept at learning complex temporal dependencies.
- Daily price data for GME in 2021 was obtained using yfinance API.
- The aim was to train LSTM models to predict the next day's closing price based on historical data.

## Data:
- Daily open, high, low, close, volume data for GME stock in 2021 was downloaded.
- Close price was selected as the prediction target and normalized.
- Input features comprised the normalized close price over the last 10 days.

## Methodology:
- LSTM models with 1 or 2 layers were constructed using PyTorch.
- Models were trained to minimize MSE loss using Adam optimizer.
- Models were trained for 500 epochs with a batch size of 10.
![AdamW](https://github.com/Santhoshkumar-p/stock-prediction/assets/24734488/e1509bcd-5128-4aae-89e7-d6f851d3dc2d)

## Results:
- The 1-layer LSTM model achieved a validation RMSE of 0.024, while the 2-layer model achieved 0.021.
- Models demonstrated the feasibility of using LSTMs for stock prediction.
### Predictions with Sentiment Analysis
![Inference - Stock Prediction with sentiment analysis](https://github.com/Santhoshkumar-p/stock-prediction/assets/24734488/9b6bfec7-43fd-4ef1-9183-a16d0d46904a)
### Negative Sentiment Analysis and Stock Price Correlation
![Inference - Negative Sentiment Analysis](https://github.com/Santhoshkumar-p/stock-prediction/assets/24734488/5d1f15a7-0bae-4c1a-a85c-b8bffda37cfb)
### Positive Sentiment Analysis and Stock Price Correlation
![Inference Sentiment Analysis Positive](https://github.com/Santhoshkumar-p/stock-prediction/assets/24734488/868edd50-5106-4832-a418-0bf18e6eeb5a)
### Confusion Matrix(Ground Truth Vs Prediction)
![Confusion Matrix FInal](https://github.com/Santhoshkumar-p/stock-prediction/assets/24734488/9bf1448b-08c8-4989-9e43-b1e3ff60c10d)

## Conclusion:
This project showcased the effectiveness of LSTM networks in modeling temporal patterns in stock prices. Future enhancements could include incorporating additional features like technical indicators and sentiment analysis to further improve predictions.

