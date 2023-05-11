# Exponential Smoothing

Exponential smoothing is a set of techniques commonly used in time series analysis to forecast future values of that same series. It is a prediction technique that uses a weighted average of past observations, with weights decreasing exponentially as the observations become older.

There are different models of exponential smoothing, such as Simple Exponential Smoothing, Holt's Exponential Smoothing, and Holt-Winters' Exponential Smoothing. Concepts such as trend and seasonality are important in deciding which exponential smoothing model to use.

***

## Trend and Seasonality

Trend and seasonality are two important concepts in time series analysis that help to understand the behavior of the series over time.

Trend refers to the overall direction of the series over time, that is, whether the series is increasing, decreasing, or remaining relatively stable. The trend can be linear, when the series increases or decreases steadily over time, or nonlinear, when the series shows more abrupt changes in direction.

Seasonality, on the other hand, refers to repetitive patterns in the series that occur at regular intervals, usually associated with seasonal events such as seasons of the year or holidays. For example, ice cream sales may exhibit seasonality in a tropical country, with higher demand during the summer and lower demand during the winter.

Understanding the trend and seasonality of a series is important for choosing the appropriate model for time series analysis and forecasting, as different models are more suitable for different patterns of time series. Additionally, identifying these patterns can help make informed decisions based on the information extracted from the series.

### Example

Decomposing the following randomly generated time series into trend and seasonality terms:

![alt text](https://github.com/Andrercouto/TimeSeriesAnalysis/blob/main/Img/rand.png?raw=true)

As shown in the image below, the random series clearly has an upward trend over time:

![alt text](https://github.com/Andrercouto/TimeSeriesAnalysis/blob/main/Img/rand-trend.png?raw=true)

Also, a pattern of constant peaks and valleys can be easily observed, which is the seasonality of the series:

![alt text](https://github.com/Andrercouto/TimeSeriesAnalysis/blob/main/Img/rand-seas.png?raw=true)

***

## Exponential Smoothing Models

- Simple Exponential Smoothing

	The simple exponential smoothing model is a technique used in time series analysis to predict future values based on historical data. The idea behind exponential smoothing is that the predicted value is a weighted combination of historical values, with weights that decrease exponentially as the data gets older.

- Holt Exponential Smoothing

	The Holt Linear Exponential Smoothing model, also known as Holt, is an extension of the Simple Exponential Smoothing model (SES) that allows for capturing trends in the data. The model is called "linear" because it uses a linear function to estimate the trend.

- Holt-Winters Exponential Smoothing

	The Holt-Winters Exponential Smoothing model is an extension of the Holt model to include seasonal components. It is used to make predictions for time series with trend and seasonality.

	The Holt-Winters model can be used in two variations: additive and multiplicative. The additive variation is used when the magnitude of the seasonal variation is constant, while the multiplicative variation is used when the magnitude of the seasonal variation is proportional to the level of the series. The choice between the two variations depends on the analysis of the time series and the characteristics of the seasonality.
