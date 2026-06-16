# Crude Oil Production Forecasting Using Machine Learning and Time Series Models

## Overview

This project focuses on forecasting U.S. crude oil production using historical monthly production data obtained from the U.S. Energy Information Administration (EIA). The objective is to compare traditional statistical forecasting methods with modern machine learning approaches and identify the most effective model for production prediction.

The project includes data preprocessing, feature engineering, stationarity analysis, model development, performance evaluation, and future forecasting.

## Features

* Historical crude oil production analysis
* Feature engineering using lag variables and rolling averages
* Stationarity testing using the Augmented Dickey-Fuller (ADF) test
* Time Series Cross-Validation
* Multiple forecasting models:

  * Linear Regression
  * Random Forest Regressor
  * XGBoost Regressor
  * ARIMA
  * Linear Regression + XGBoost Hybrid Model
* Future production forecasting through 2031
* Model comparison using MAE, RMSE, and R² Score

## Dataset

Source: U.S. Energy Information Administration (EIA)

Period Covered: 1980–2026

Target Variable:

* Monthly Crude Oil Production

Engineered Features:

* Month
* Year
* lag_1
* lag_3
* lag_6
* lag_12
* rolling_mean_3
* rolling_mean_6
* rolling_mean_12

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Statsmodels

## Results

| Model                              | R² Score |
| ---------------------------------- | -------: |
| Linear Regression                  |   0.8809 |
| Linear Regression + XGBoost Hybrid |   0.8765 |
| Random Forest                      |  -1.0446 |
| XGBoost                            |  -1.1561 |
| ARIMA                              |  -4.5557 |

Linear Regression achieved the best performance and was selected as the final forecasting model.

## Future Forecasting

Using the best-performing model, crude oil production forecasts were generated for the period 2026–2031. The results indicate a continued upward trend in future production levels.

## Author

Khushi Singh

B.Tech Computer Science and Engineering

SRM Institute of Science and Technology
