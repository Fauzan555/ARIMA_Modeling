# This repository provides a practical, step-by-step guide for implementing time series analysis using ARIMA modeling. The main focus is on forecasting climate variables such as mean temperature and humidity, using Python and popular data science libraries.

# Table of Contents
Overview

Dataset

Workflow

ARIMA Modeling Steps

How to Run

Results

Dependencies

References

# Overview

Time series analysis is a powerful technique for analyzing data points collected or recorded at specific time intervals. The ARIMA (AutoRegressive Integrated Moving Average) model is a classic method for forecasting such data. This repository demonstrates:

Exploratory Data Analysis (EDA) on climate data

Stationarity checks

Parameter selection for ARIMA

Model training, evaluation, and forecasting

Hyperparameter tuning using grid search

# Dataset

# Sources  https://www.kaggle.com/datasets/sumanthvrao/daily-climate-time-series-data
The notebook uses the DailyDelhiClimateTest.csv dataset, which contains columns like:

date
meantemp

humidity

wind_speed

meanpressure

# Workflow

The notebook Implement ARIMA Modeling.ipynb follows these steps:

# 1 Data Loading and Visualization:

Read the CSV data into a pandas DataFrame.

Plot trends for temperature and humidity over time.

Explore correlations between variables.

# 2 Stationarity Check:

Use the Augmented Dickey-Fuller (ADF) test to check if the time series is stationary.
If not stationary, apply differencing and visualize the results.

# 3 Model Parameter Identification:

Plot Autocorrelation (ACF) and Partial Autocorrelation (PACF) to help pick the best ARIMA parameters (p, d, q).

# 4 Model Fitting:

Fit ARIMA models to the time series data (mean temperature, humidity).

Print model summaries and diagnostics.

# 5 Evaluation and Forecasting:

Visualize actual vs. fitted values.

Forecast future values (e.g., next 15 days).

# 6 Hyperparameter Tuning (Grid Search):

Search over different ARIMA configurations.

Select the best model based on Mean Squared Error (MSE).

# ARIMA Modeling Steps

AR (AutoRegressive): Uses past values to predict the future.

I (Integrated): Applies differencing to make the series stationary.

MA (Moving Average): Uses past forecast errors.

The model is typically written as ARIMA(p, d, q).

# How to Run

Clone the repository:


git clone https://github.com/Fauzan555/Guide_on_time_series_analysis.git

# cd Guide_on_time_series_analysis

# Install dependencies (see below).

# Ensure the dataset (e.g., DailyDelhiClimateTest.csv) is in place.

# Run the notebook:


jupyter notebook "Implement ARIMA Modeling.ipynb"


# Results

The best ARIMA configuration for mean temperature and humidity is typically found via grid search.

Model evaluation plots and forecast values are integrated into the notebook.

Example output (from grid search):


# Best ARIMA config for mean temperature : (3, 1, 3) with MSE=2.650

# Best ARIMA config for humidity feature: (3, 1, 3) with MSE=44.166

# Dependencies

Install these packages before running the notebook:

pandas

numpy

matplotlib

seaborn

statsmodels

scikit-learn


# References

ARIMA Model - Wikipedia

Statsmodels Documentation

Time Series Analysis with Python
