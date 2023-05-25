
## Determining Car Price Based on Available Features

### Toolkit

Data preprocessing: handling missing values and duplicates, changing data types, grouping tables;  
Applying standard prediction models and gradient boosting models: sklearn, LightGBM, XGBoost, CatBoost;  
Checking results on validation and test samples.  
### Introduction
The project task is to build a model for determining the cost of a car for a used car sales service that is developing an application to attract new customers. We have the following data at our disposal: technical specifications, configurations, and car prices.  
The customer is interested in:

  * prediction quality;
  * prediction speed;
  * training time.

### Goal 
Creation of a model that predicts the price of a car based on certain features.  
There is labeled data: car characteristics and sales price.

### Project Structure
1. Loading and processing data: filling in missing values, grouping by features, finding duplicates, visualizing results;  
2. Training gradient boosting models, analyzing learning speed;  
3. Training prediction models requiring dummy transformation - linear regression, random forest.  
4. Model validation and selection of the best.  

### Overall Conclusion 
- Five models participated in the study: 'LightGBM', 'Catboost', 'Gradient_Boosting', 'LinearRegression', 'RandomForestRegressor'. 
- The main testing metric was the RMSE metric.  
- In the first stage of the study, data analysis was performed and missing values were filled in.  
- In the second stage of work, 5 forecasting models were tested.  
- The best and recommended model for use was recognized as LightGBM - with an RMSE value on the test sample = 1654.23, training time = 1.5  minutes, prediction time 10 sec on the training server.  
