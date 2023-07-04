# Gas-Prices

Our objective in this study is to build models based on the time-series dataset of the Henry Hub natural gas price and create a two-year forecast by using different time series models in R programming. 

# Dataset Information 

The dataset is collected from [the US Energy Information Administration](https://www.eia.gov/dnav/ng/hist/rngwhhdm.htm). The dataset consists of monthly Henry Hub natural gas spot prices starting from January 1997 until March 2022. The price is denominated by US dollar Metric Million British thermal unit (US$/MMBtu). Prices are based on delivery at the Henry Hub in Louisiana. Official daily closing prices at 2:30 p.m. from the trading floor of the New York Mercantile Exchange (NYMEX) for a specific delivery month [(EIA, 2020).](https://www.eia.gov/dnav/ng/NG_PRI_FUT_S1_M.htm)

# End Result

The result can also be viewed in my Rpubs : https://rpubs.com/Fib_Gro/Gas_Price

# File Attachment 

- Rmd File
- csv File
- png File

# Conclusion 

1. All models are considered not representative of forecasting the Henry Hub gas price. The visualization of the forecast illustrates that the forecast model has a different pattern from the data test. In addition, there is a lagging in the model compared to the original data. This conclusion is also confirmed by the high forecast error of MAPE in all models.
2. Model TBATS is considered a better performance model compared to other models. However, this model still violates the normality of residual assumption.
3. Improving the model can be done by tuning the hyperparameter for each model. Such as in ETS, we could change the alpha, beta or gamma in the parameter instead of just relying on the automated function. Another suggestion is to use another model to forecast the gas price, such as GBM (Geometric Brownian Motion) or an MRP (Mean Reverting Process) that is extensively used for modelling commodities price
