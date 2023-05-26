
## Forecasting the number of taxi orders for a specific hour

### Toolkit
Time series processing, statsmodels library;  
Analysis of global trends, seasonality, daily and hourly patterns;  
Feature engineering: date decomposition, introduction of lags and moving average;  
Models from sklearn and gradient boosting - CatBoost, LightGBM.  
### Introduction
A taxi aggregator is analyzing patterns in daily orders to attract more drivers during peak hours.  
We have labeled data: the number of orders every hour over several months.  
### Goal
Build a model to forecast the number of orders each hour. The prediction time and RMSE metric should be minimal.  

### Project structure 
1. Data exploration and preprocessing;
2. Data analysis: trends, seasonality, data type, anomaly detection;
3. Model training:
   * Feature creation;
   * Splitting the data into a training set and a target set;
   * Model training and hyperparameter tuning;
4. Testing of the best model;
5. Conclusion.

### General conclusion
This project involved analyzing data about taxi orders at airports.

Key findings include:
* There is an overall trend of increasing taxi orders from month to month;
* Taxis are most frequently ordered on Mondays and Fridays, due to a higher number of flights over the weekend;
* Taxis are most commonly ordered around midnight, likely because the Aeroexpress trains are not operational at this time, forcing people to order taxis to get home;

* The LGBMRegressor model delivered the best RMSE result, at 42.75. However, the GradientBoostingRegressor model operates almost twice as fast, with a not significantly higher RMSE.

Future work could involve both models, choosing the best one depending on whether speed or accuracy is more important.
