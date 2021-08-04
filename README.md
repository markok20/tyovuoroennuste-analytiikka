# Forecasting workflow volumes

The intention is to build a forecast model of incoming calls to the contact center.

The goal is to optimize customer service resourcing.

The challenge:

If AsPa has too few resources, there will be queuing and customer dissatisfaction. Underlying SLA requirements.

If AsPa has too many people, unnecessary staff costs, there is nothing useful to do.

The number of incoming Calls / Feedback to AsPaa varies seasonally.

Other marketing factors e.g. various campaigns and other events increase the number of daily customer contacts, which is not taken into account by historical data. This must be taken into account in the forecast.

Time series forecasting of demand by machine learning method, programming language Python

By forecasting the daily / weekly / monthly volumes of calls and e-mails to customer service, customer service can be resourced more optimally.

Historical data available on the number of calls and messages over a sufficient time cycle. Qualitative customer interviews can also provide information from other sources, including marketing factors and cyclical fluctuations.

The challenge is that historical data produces overly subjective estimates. In addition to historical information, interviews on unforeseen marketing factors.

Time series forecasting is time-bound regularity.

The time series can be divided into components, which are trend, seasonal variation, cyclical variation, and random variation.

Central to modeling is parameter estimation.

The moving average is the simplest model to predict development.

In the moving average method, the forecast of future time demand is the average of the demand of past times.

As a solution: exponential smoothing (moving average weighted to the most recent times) => The forecast is sensitive to changes and easy to update.

One of the most popular models for demand forecasting.

Components that take into account trend and seasonality can be added to the model.

In addition to the basic level of demand, factors affecting demand include trend, seasonal, cyclical and marketing factors as well as unpredictable fluctuations.

The model can also be used to predict other contact center data.

Simple, double (Holt model) and triple (Holt-Winter model) exponential smoothing models.

Exponential smoothing can be found in the statsmodels.tsa library.

The triple model takes into account both trend and seasonality.
