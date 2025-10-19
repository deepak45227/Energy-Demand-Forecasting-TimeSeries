
# Energy Demand Forecasting

## Objective: A utility company wanted to predict the electricity demand accurately to optimize power generation and distribution.

## Approach: Time series data from past years, including historical demand, weather data, and holidays, was collected. SARIMA and Prophet models were used to capture seasonality and trends. DeepAR was applied for probabilistic forecasting with prediction intervals.

## Outcome: The accurate forecasts enabled the utility company to optimize power generation, reduce operational costs, and prevent energy shortages during peak demand periods.















The plot shows both the load and solar generation over time for the year 2016. The load appears to have a cyclical pattern with peaks and valleys, possibly corresponding to daily patterns of electricity use.
The solar generation also shows a clear pattern, with generation during the day and no generation at night (as expected). The amount of solar generation also appears to fluctuate throughout the year, likely due to seasonal changes in sunlight.
Before moving on to time series analysis and forecasting with ARIMA, it's important to check for stationarity in your time series data. Stationarity is a property of time series data that implies the mean, variance, and autocorrelation structure do not change over time. Many time series models, including ARIMA, require the data to be stationary.
Let's perform an Augmented Dickey-Fuller test to check the stationarity of the time series. The null hypothesis of the ADF test is that the time series is non-stationary. So, if the p-value of the test is less than the significance level (0.05) then you reject the null hypothesis and infer that the time series is indeed stationary.