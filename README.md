Task 14: Time Series Analysis
Edutech Solution — Data Science Internship

Overview
Time series analysis on the AirPassengers dataset to decompose trends, test stationarity, and forecast future values using SARIMA.

Dataset
AirPassengers — Monthly international airline passengers (1949–1960), 144 observations


Steps Performed
Decomposition — Separated the series into Trend, Seasonality, and Residual using a multiplicative model
Stationarity Test — Applied ADF test; achieved stationarity after log transform + d=1 + D=1
ACF/PACF Analysis — Identified model order: p=1, q=1, P=1, Q=1
SARIMA Model — Fitted SARIMA(1,1,1)(1,1,1,12); AIC = -427.03, MAPE = 14.11%
Forecast — Predicted 24 months ahead (Jan 1961 – Dec 1962) with 95% confidence intervals

Results

Metric                    Value
Model                     SARIMA(1,1,1)(1,1,1,12)
AIC                       -427.03
MAPE                       14.11%
Forecast Peak             ~679 passengers (Jul 1961)
