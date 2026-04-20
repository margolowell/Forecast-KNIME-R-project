# Forecast-KNIME-R-project

## Time Series Forecasting Project

## About

Individual project focused on forecasting real-world time series data using KNIME and R, with an emphasis on model evaluation and practical application to demand planning.

## Overview

This project focuses on forecasting U.S. air passenger demand using monthly time series data from FRED (AIRRPMTS). The goal is to develop an accurate forecasting model to support demand planning decisions such as flight scheduling and staffing.

The analysis emphasizes model selection, validation, and interpretability through a combination of KNIME workflows and R-based time series modeling.

## Project Structure

The project is organized into several stages of the forecasting workflow:

Data Preparation: Importing and converting FRED data into a time series format
Exploratory Analysis: Identifying trends, seasonality, and structural changes (e.g., COVID-19 impact)
Model Development: Building and comparing multiple forecasting models
Model Evaluation: Using time series cross-validation (TSCV) and error metrics to assess performance
Forecasting: Generating a 12-month forecast for demand planning

## Tools Used
- KNIME
- R (via KNIME R Snippet & R View nodes)
- fpp3 / forecast packages

## Models Implemented
- Seasonal Naive (SNaive)
- Drift
- ARIMA (1, 1, 1)
- ARIMA (1,1,0)
- SARIMA (1,1,0) (1,0,0) [12]
- ETS (A, A, A)

## Key Skills Demonstrated
- Time series analysis and forecasting
- Stationarity testing (ADF test)
- ACF/PACF interpretation
- ARIMA/SARIMA model development
- Time series cross-validation (TSCV)
- Model evaluation using RMSE, MAE, and MASE
- Residual diagnostics and model validation
- Integrating KNIME workflows with R

## Results

The SARIMA model was selected as the final model based on superior performance in time series cross-validation. It achieved significantly lower forecast errors compared to benchmark models, with a MASE of 0.59, indicating approximately 41% lower error than a naive approach.

A 12-month forecast was generated, capturing both seasonal patterns and overall demand trends.

## What I Learned
- How to apply end-to-end time series forecasting in a structured workflow
- The importance of balancing model diagnostics with predictive performance
- How seasonality and external shocks (e.g., COVID-19) impact forecasting models
- How to use cross-validation to make more reliable model selection decisions

