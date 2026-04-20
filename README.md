# BAJAJFINSV Stock Price Analysis and ARIMA Forecasting

This notebook performs a comprehensive time-series analysis on BAJAJFINSV equity data to predict future closing prices.

## Project Overview
1. **Data Preprocessing**
   - Cleaned column names and handled date formatting.
   - Converted price strings (with commas) to numeric floats.
   - Verified data integrity (no missing values found).

2. **Exploratory Data Analysis**
   - Visualized the historical closing price trend to identify volatility and underlying patterns.

3. **ARIMA Modeling**
   - **Stationarity**: Performed the Augmented Dickey-Fuller (ADF) test, which confirmed the series was non-stationary ($p > 0.05$).
   - **Parameters**: Used ACF and PACF plots to identify optimal lags. Fitted an ARIMA(1, 1, 1) model.
   - **Evaluation**: The model was validated on a test set, achieving an RMSE of approximately 150.93.

4. **Future Forecast**
   - Predicted the next 30 days of closing prices.
   - **Interpretation**: The model predicts a period of **stability and consolidation** following recent volatility, with prices 
