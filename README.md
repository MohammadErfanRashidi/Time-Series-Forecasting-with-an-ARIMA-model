# Stock Price Forecasting with ARIMA

This project demonstrates how to forecast stock prices using the ARIMA (Autoregressive Integrated Moving Average) model in Python. It uses the `yfinance` library to download historical stock data and `statsmodels` for the ARIMA implementation.

## Steps:

1. **Install necessary libraries:**
   
3. **Import libraries:**
   
4. **Load and visualize data:**
   - Downloads historical stock data for Apple (AAPL) from Yahoo Finance.
   - Plots the closing price over time.

5. **Check for stationarity:**
   - Uses the Augmented Dickey-Fuller (ADF) test to check if the time series is stationary.
   - If not stationary, applies differencing to make it stationary.

6. **Identify model order using ACF and PACF:**
   - Plots the Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) to help determine the order (p, d, q) for the ARIMA model.

7. **Fit ARIMA model:**
   - Creates and fits an ARIMA model with the chosen order.
   - Prints the model summary.

8. **Forecast and evaluate:**
   - Generates in-sample predictions (one-step-ahead forecasts).
   - Plots actual vs. predicted prices.
   - Calculates the Mean Absolute Error (MAE) to evaluate the model's performance.

9. **Analyze residuals:**
   - Plots the residuals to assess model fit.
   - Calculates the MAE of the residuals.


## Note:

- The code uses Apple (AAPL) as an example. You can change the ticker symbol to forecast other stocks.
- The ARIMA model's order may need to be adjusted for different stocks and time periods.
- This is a basic example and can be extended with more features and analysis for improved forecasting accuracy.
