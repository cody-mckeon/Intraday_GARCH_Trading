# Intraday_GARCH_Trading
This project implements an intraday trading strategy using a GARCH (Generalized Autoregressive Conditional Heteroskedasticity) model.

This project implements an intraday trading strategy using a GARCH (Generalized Autoregressive Conditional Heteroskedasticity) model. The strategy is based on simulated daily and intraday 5-minute data. The goal is to predict daily volatility using a GARCH model, generate a trading signal based on this prediction, and then refine the signal using intraday indicators to execute trades. The final output is the calculation of strategy returns.

# Project Overview

The project follows a structured approach to develop and test an intraday trading strategy:

# Data Loading: 
Load simulated daily and intraday (5-minute) data from CSV files.
- **GARCH Model Fitting**: Define and fit a GARCH model on daily data to predict 1-day ahead volatility using a rolling window approach.
- **Prediction Premium Calculation**: Calculate a prediction premium from the GARCH model output and form a daily trading signal.
- **Intraday Signal Formation**: Merge the daily signal with intraday data and calculate additional intraday indicators to refine the trading signal.
- **Position Entry and Exit**: Generate trading positions based on the intraday signal and hold these positions until the end of the day.
- **Strategy Returns Calculation**: Calculate the final strategy returns based on the generated positions.
# Key Features

# GARCH Model Implementation: 
- **GARCH Model Implementation**: Use the `arch` library to fit a GARCH model on daily returns and predict future volatility.
- **Intraday Data Integration**: Combine daily volatility predictions with intraday data to generate refined trading signals.
- **Rolling Window Predictions**: Implement a rolling window to continuously update the model and predictions based on the latest data.
- **Strategy Backtesting**: Backtest the intraday strategy to evaluate its performance over the simulation period.
