## Algorithm Understanding
* <i> How does the Prophet Algorithm differ from an LSTM? </i>
The prophet algorithm is decomposable additive model with components for modelling the trend/growth, seasonality and holidays, and is specifically targetted for time series. It uses a combination of regression and Fourier series. 
LSTMS, on the other hand, are deep neural networks based on recurrent neural networks, and can be applied to any sequential data including time series. 

* <i> Why does an LSTM have poor performance against ARIMA and Prophet for Time Series? </i> LSTMs may have poorer performance than ARIMA and Prophet for time series if the amount of data is not large, and the data has clear seasonality & trends that can be easily captured with ARIMA and Prophet. 
But for larger datasets, LSTMs have been shown to perform better in capturing any non-linear trends in the time series data (<url>https://arxiv.org/pdf/2107.12770.pdf</url>)

## Interview Readiness
* <i>What is exponential smoothing and why is it used in Time Series Forecasting?</i>
Exponential smoothing is a time series forecasting method that uses weighted sum of past observations to make predictions for future. The weighting is performed such that more recent observations are weighted higher than earlier ones.
Single exponential smoothing is used for forecasting in data without any seasonality or trend, with a single hyperparameter <i>alpha</i>, smoothing coefficient. 
With double and triple smoothing, additional support for trend and seasonality is added. 


* <i>What is stationarity? What is seasonality? Why Is Stationarity Important in Time Series Forecasting?</i>
Stationarity in time series refers to the property of the series to keep its statistical attributes (mean, variance, autocorrelation) constant. This means that the time series does not have trend or seasonality. 
Trend is a property of time series in which the observations are steadily increasing, decreasing or flat over time. 
Seasonality in time series refers to regular patterns like daily, weekly, monthly etc. or due to seasons, holidays etc. 
Stationarity is important in time series forecasting because techniques such as exponential smoothing and ARIMA assume that the time series has stationarity. 

* <i>How is seasonality different from cyclicality? Fill in the blanks: ___ is predictable, whereas ___ is not. </i>
Seasonality refers to patterns correlated with time of the year - for instance, higher consumer buying patterns in winter. Here the time period is fixed and known, and hence predictable. 
Cyclicality on the other hand, refers to rises and falls in data that are not of fixed time period - for instance, higher purchase patterns when unemployment rates are lower. Although the patterns tend to repeat, the durations are longer and not predictable.
Seasonality is predictable whereas cyclicality is not. 
