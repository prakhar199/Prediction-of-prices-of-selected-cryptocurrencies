# Prediction-of-prices-of-selected-cryptocurrencies-using-the-ARIMA-and-SARIMAX-model.

Cryptocurrencies that have been analyzed:
Bitcoin,
More will be released soon.
Project Overview
ARIMA (Auto Regressive Integrated Moving Average) is a combination of 2 models: AR (Auto Regressive) and MA (Moving Average).
It has 3 hyperparameters:

p (auto regressive lags)
d (order of differentiation)
q (moving average)
which respectively comes from the AR, I and MA components.

The AR part is correlation between previous and current time periods. To smooth out the noise, the MA part is used.
The I part binds together the AR and MA parts.

If we want to find value of P and Q for ARIMA model, we need to take ACF (Auto Correlation Function) and PACF (Partial Auto Correlation Function) plots. We need to check, for which value in x-axis, graph line drops to 0 in y-axis for the first time.

From PACF (at y=0), get P.
From ACF (at y=0), get Q.
An ADF test (Augmented Dickey–Fuller) tests the null hypothesis that a unit root is present in a time series sample. The alternative hypothesis is different depending on which version of the test is used, but is usually stationarity or trend-stationarity. It is an augmented version of the Dickey–Fuller test for a larger and more complicated set of time series models. The augmented Dickey–Fuller statistic, used in the test, is a negative number. The more negative it is, the stronger the rejection of the hypothesis that there is a unit root at some level of confidence.

➡️ p value (where 0 ≤ p ≤ 1) should be as low as possible. Critical values at different confidence intervals should be close to the Test statistics value.
