# R-Project-1-Forecasting-10yr-Market-Yields

This is a current ongoing modeling project in R.

Project 1: Forecasting 10-Year US Treasury Security Yields
Introduction
This project focuses on forecasting the yields of 10-year US Treasury securities using time series analysis in R. The aim is to apply various statistical models to understand and predict the behavior of these yields, which are pivotal in the financial sector.

Data Source
The primary dataset used is the Market Yield on U.S. Treasury Securities at 10-Year Constant Maturity, quoted on an investment basis, sourced from Federal Reserve Economic Data (FRED).

Setup and Data Preparation
Initial steps involve setting up the R environment with necessary packages (forecast, zoo, ggplot2, dplyr, xts, lubridate, tseries) and preparing the data by reading and cleaning it to ensure quality analysis.

Data Exploration
In-depth data exploration includes:

Visualization of the original data to understand its nature and behavior.
Conducting the Augmented Dickey-Fuller (ADF) test to check for stationarity.
Examining various aspects like trends, seasonality, noise, and volatility in the data.
Time Series Decomposition
The time series is decomposed to analyze its components and check for the presence of seasonality.

Forecasting Models
Two primary models are used for forecasting:

Exponential Smoothing (Holt-Winters method): Applied to the data without a gamma component, considering the sum of squared errors and visualizing the forecasts.
ARIMA (AutoRegressive Integrated Moving Average): Utilizing auto.arima to identify the best-fitting model, log-transforming the data for stationarity, and examining ACF and PACF plots to determine the ARIMA model parameters.
Model Evaluation
The models are assessed based on their fit to historical data and forecast accuracy.
Residual analysis is conducted to check the adequacy of model fitting.
Ljung-Box tests are performed to evaluate the lack of fit.
Time Series Cross-Validation
Comparative analysis between auto.arima and ets methods is carried out to determine the more effective model for this dataset.

Back-Testing
Back-testing is conducted to evaluate the model's performance on historical data, split into training and test sets, to gauge its predictive capability.
