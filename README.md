# Time-Series-Forecasting

# Introduction
Time series forecasting is a difficult problem with no easy answer. There are countless statistical models that claim to outperform each other, yet it is never clear which model is best.

That being said, ARMA-based models are often a good model to start with. They can achieve decent scores on most time-series problems and are well-suited as a baseline model in any time series problem.

## Autoregressive Integrated Moving Averages
The ARIMA model acronym stands for “Auto-Regressive Integrated Moving Average” and for this article we will will break it down into AR, I, and MA.

The general process for ARIMA models is the following:
* Visualize the Time Series Data
* Make the time series data stationary
* Plot the Correlation and AutoCorrelation Charts
* Construct the ARIMA Model or Seasonal ARIMA based on the data
* Use the model to make predictions

### Final Thoughts on Autocorrelation and Partial Autocorrelation

* Identification of an AR model is often best done with the PACF.
    * For an AR model, the theoretical PACF “shuts off” past the order of the model.  The phrase “shuts off” means that in theory the partial autocorrelations are equal to 0 beyond that point.  Put another way, the number of non-zero partial autocorrelations gives the order of the AR model.  By the “order of the model” we mean the most extreme lag of x that is used as a predictor.   
* Identification of an MA model is often best done with the ACF rather than the PACF.
    * For an MA model, the theoretical PACF does not shut off, but instead tapers toward 0 in some manner.  A clearer pattern for an MA model is in the ACF.  The ACF will have non-zero autocorrelations only at lags involved in the model. 
    p,d,q
    p AR model lags
    d differencing
    q MA lags

# Final Forecasted Sales for next two years
![Output](https://github.com/ShubhiGupta15/Time-Series-Forecasting/assets/79734129/c10704c0-374b-4dcb-b1b8-e4bf794bf6cd)


