# ARIMA Modeling

ARIMA (AutoRegressive Integrated Moving Average) is another powerful technique in time series analysis for forecasting future values. It combines autoregressive, moving average, and differencing components to capture different patterns and dependencies present in the data.

ARIMA models are effective in handling both trend and seasonality in time series data. By incorporating lagged observations, moving averages, and differencing, ARIMA models can capture the underlying patterns and make accurate predictions.

***

## Main Components

ARIMA models consist of three main components: autoregressive (AR), integrated (I), and moving average (MA). These components are combined to capture different patterns and dependencies present in the time series data.

- Autoregressive (AR) Component: The autoregressive component models the relationship between the current observation and a specified number of lagged observations. It assumes that the current value of the time series is dependent on its previous values. The "p" parameter in ARIMA(p, d, q) represents the order of the autoregressive component.

- Integrated (I) Component: The integrated component accounts for the differencing required to make the time series stationary. Stationarity is a desirable property in time series analysis, as it ensures that the statistical properties of the series do not change over time. The "d" parameter in ARIMA(p, d, q) represents the order of differencing applied to the time series.

- Moving Average (MA) Component: The moving average component models the dependency between the current observation and a specified number of lagged forecast errors. It captures the random shocks or noise present in the time series. The "q" parameter in ARIMA(p, d, q) represents the order of the moving average component.

By combining these components, ARIMA models can capture various patterns in time series data, such as trend, seasonality, and random fluctuations. The order of the components (p, d, q) in an ARIMA model is determined based on the characteristics observed in the data and is selected using techniques like model diagnostics, information criteria, or grid search.

## Stationarity

Stationarity is an essential condition for the application of ARIMA models. A stationary process is one in which statistical properties, such as mean and variance, remain constant over time. Stationarity is important because ARIMA models assume that the time series is stationary or can be transformed into a stationary series.

The main reasons for the need for stationarity are the stability of statistical properties since ARIMA models assume that the statistical properties of the series, such as mean and variance, remain constant over time, and a well-defined autocorrelation among the values, meaning that the dependence between past and future values is consistent.

The stationarity of a series can be tested through the Dickey-Fuller test, widely used in time series analysis. The test is based on the null hypothesis that the time series has a unit root, indicating non-stationarity. The aim of the test is to determine if there is sufficient evidence to reject this null hypothesis and conclude that the series is stationary by comparing the difference between consecutive observations of the series with a critical value for determining the presence of a unit root.