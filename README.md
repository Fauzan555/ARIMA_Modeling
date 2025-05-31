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
