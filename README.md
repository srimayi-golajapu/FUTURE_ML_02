# FUTURE_ML_02
Built a time-series sales forecasting system using historical business data to predict future daily demand. Applied time-aware data preparation, seasonal feature engineering, regression-based forecasting, and clear visualizations to support inventory planning, staffing, and business decision-making

Title
Sales Demand Forecasting Using Time Series Analysis

Project Overview
This project builds a sales demand forecasting system using historical business data.
The goal is to predict future sales trends and present the results in a clear, business-friendly way that supports inventory planning, staffing decisions, and cash flow management.

Instead of focusing only on model accuracy, the project emphasizes proper time-series handling, interpretability, and practical business insights.

Problem Statement
Businesses need reliable sales forecasts to plan operations and reduce risk.
Manual forecasting is slow and inconsistent, while naive models often ignore seasonality and trends.

This project addresses the problem by forecasting future daily sales using past sales patterns.

Dataset
The project uses historical sales data containing:

Date of sales

Sales or demand values

The approach is dataset-agnostic and can be applied to any time-based sales dataset.

Approach
The forecasting pipeline follows a real-world machine learning workflow:

Data loading and inspection

Time-based data preparation

Aggregation of daily total sales

Chronological train–validation split

Time-based feature engineering

Baseline forecasting using Linear Regression

Model evaluation using MAE and RMSE

Visualization of actual vs forecasted sales

Business interpretation of results

Random train-test splitting is avoided to prevent time leakage.

Feature Engineering
Time-based features extracted from the date column include:

Day of week

Day of month

Month

Week of year

These features help the model learn seasonality and recurring demand patterns.

Model Used

Linear Regression

A simple and interpretable baseline model is used to:

establish a reliable benchmark

ensure explainability for business stakeholders

More complex models can be added later if required.

Evaluation Metrics

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

MAE is emphasized as it represents average daily forecast error in business terms.

Results
The model successfully captures:

overall sales trends

recurring seasonal patterns

Forecast results are visualized to clearly compare:

historical sales

actual validation sales

predicted future sales

This visualization makes the forecast easy to understand for non-technical users.

Business Use Case
The forecast can be used by businesses to:

plan inventory levels

reduce stockouts and overstocking

schedule staff based on expected demand

estimate short-term cash flow

Limitations

Promotions, holidays, and external shocks are not explicitly modeled

Forecast accuracy may decrease during unexpected events

These limitations are expected for a baseline model.

Tools and Technologies

Python

Pandas

NumPy

Scikit-learn

Matplotlib

Jupyter Notebook

How to Run

Clone the repository

Install required libraries

Run the notebook step by step

View forecast plots and evaluation metrics

Future Improvements

Add lag and rolling window features

Include holiday and promotion data

Experiment with advanced forecasting models

Deploy as a forecasting dashboard
