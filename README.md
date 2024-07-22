# Time-Series-Analysis-of-Australia-Unemployment-Rate
This repository contains code and analysis for predicting Australia's unemployment rate using time series analysis techniques. The project focuses on modeling and forecasting the monthly unemployment rate for Australians aged 15-24 from 2002 to 2011 using various SARIMA models.


## Introduction
This project analyzes the monthly unemployment rate of Australians aged 15-24 from 2002 to 2011. The analysis identifies trends, seasonality, and other characteristics of the time series data to build predictive models.

## Dataset
The dataset includes the unemployment rate measured monthly. The analysis uses data from November 2002 to October 2011, focusing on the significant change points influenced by economic events.

## Methodology


**Data Preprocessing:** Scripts and notebooks for cleaning and preparing the unemployment rate data. 
**Exploratory Data Analysis (EDA):** Visualizations and statistical analyses to understand the data's underlying patterns.
**Stationarity Tests:** Implementation of Augmented Dickey-Fuller (ADF), Phillips-Perron (PP), and Kwiatkowski-Phillips-Schmidt-Shin (KPSS) tests to check for stationarity.
**Model Identification:** Use of Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) plots to identify potential SARIMA models.
**Model Fitting:** Code for fitting various SARIMA models to the data.
**Model Validation and Diagnostics:** Scripts for validating the models and checking diagnostic plots to ensure adequacy.
**Forecasting:** Implementation of the best-fit SARIMA model to forecast future unemployment rates.
**Performance Evaluation:** Evaluation of model performance using metrics such as Mean Error (ME), Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), Mean Percentage Error (MPE), Mean Absolute Percentage Error (MAPE), Mean Absolute Scaled Error (MASE), and Autocorrelation Function of residuals at lag 1 (ACF1).

### Models Used
Several SARIMA models were evaluated, including:

* SARIMA(0,1,1)x(0,1,0)_12
* SARIMA(1,1,2)x(0,1,0)_12
* SARIMA(1,1,1)x(0,1,0)_12
* SARIMA(0,1,2)x(0,1,0)_12
* SARIMA(2,1,0)x(0,1,0)_12
* SARIMA(3,1,2)x(0,1,0)_12
* SARIMA(2,1,3)(1,1,0)_12
* SARIMA(2,1,3)(0,1,0)_12


## Results
The model **SARIMA(2,1,3)(0,1,0)_12** was selected as the best model for forecasting. The forecast includes a 10-month prediction with 80% and 95% confidence intervals.

Usage
To run the analysis, follow these steps:

Clone the repository.
Install the necessary packages.
Run the provided Jupyter notebooks or R scripts.
