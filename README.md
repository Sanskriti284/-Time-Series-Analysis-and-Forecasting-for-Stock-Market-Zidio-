# -Time-Series-Analysis-and-Forecasting-for-Stock-Market-Zidio-
A practical project on time series forecasting using real stock market data. Applied preprocessing, EDA, and models like ARIMA, SARIMA, Prophet, and LSTM to predict Apple Inc. stock prices. Evaluated with MSE, MAE, RMSE; visualized trends and seasonality. Tools: Python, Pandas, NumPy, Matplotlib, Statsmodels, TensorFlow.
Time Series Analysis and Forecasting for Stock Market
This project demonstrates practical time series forecasting using real-world stock market data. It covers data preprocessing, exploratory data analysis (EDA), and multiple models (ARIMA, SARIMA, Facebook Prophet, and LSTM) to predict stock prices for Apple Inc. Model performance is evaluated using MSE, MAE, and RMSE, with trends and seasonality visualized.

Dataset:
Source: https://www.kaggle.com/datasets/jacksoncrow/stock-market-dataset
Description: Contains historical daily prices for multiple stocks and ETFs, with Date, Open, High, Low, Close, Adjusted Close, and Volume columns.

Methods and Steps:
1. Data Preprocessing
Removed missing values and duplicates\
Converted date columns to datetime for time-indexing
Filtered relevant stocks (NASDAQ-listed, non-ETFs)
Selected Apple Inc. (AAPL) for forecasting

2. Exploratory Data Analysis (EDA)
Plotted Close and Adjusted Close prices
Calculated rolling mean and standard deviation
Applied STL decomposition for trend, seasonality, and residuals

3. Stationarity Checks
Performed ADF and KPSS tests
Applied differencing to achieve stationarity

4. Models Implemented
Naive Forecast (baseline)
ARIMA(5,2,2)
SARIMA(1,2,1)(1,0,1,7)
Facebook Prophet
LSTM Neural Network

5. Evaluation Metrics
Mean Squared Error (MSE)
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)

Results:
Model	MSE	MAE	RMSE
ARIMA(5,2,2)	83.16	5.50	9.12
LSTM	83.24	5.49	9.12
SARIMA(1,2,1)(1,0,1,7)	83.36	5.51	9.13
Naive Forecast	115.74	7.76	10.76
Facebook Prophet	32046.52	178.94	179.02

Observation:
ARIMA and LSTM models performed best. Prophet did not perform well for high-frequency stock prices.

Tools and Technologies Used: Python 3, Pandas, NumPy, Matplotlib, Seaborn, Statsmodels, Facebook Prophet, TensorFlow, Keras, Scikit-learn

Challenges
Achieving stationarity through differencing
