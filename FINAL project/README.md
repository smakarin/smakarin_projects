
# Customer Churn Prediction for Telecom Company
***

### Toolset
* Data preprocessing: handling missing values, table grouping, duplicate handling, pandas;
* Exploratory Data Analysis: seaborn and plotly;
* Applying standard forecasting models and gradient boosting models: sklearn, LightGBM, CatBoost;
* Checking the results on validation and test samples.

### Input Data

In this project, the task is to build a model that classifies users into those who are likely to switch to a competitor in the near future and those who will stay. We have the following data at our disposal: personal information about some clients, information about their tariffs and contracts.

Main metric: AUC-ROC.

Additional metric: Accuracy.

Assessment criteria:

* AUC-ROC < 0.75 — 0 sp
* 0.75 ≤ AUC-ROC < 0.81 — 4 sp
* 0.81 ≤ AUC-ROC < 0.85 — 4.5 sp
* 0.85 ≤ AUC-ROC < 0.87 — 5 sp
* 0.87 ≤ AUC-ROC < 0.88 — 5.5 sp
* AUC-ROC ≥ 0.88 — 6 sp

### Goal
To create a model that predicts customer behavior based on certain features.
There is labeled data: personal data about some customers, information about their tariffs and contracts.

### Project Structure

1. Data loading and preprocessing;


2. Exploratory data analysis:

   * Analysis of the behavior of active company clients and those who left;
   * Analysis of the dynamics of the number of new customers;
   * Analysis of the influence of payment methods on the monthly payment;
   * Analysis of the impact of the tariff (internet+phone, phone only, internet only) on the monthly payment;
   * Exploratory data analysis. Conclusion.
   
3. Creating a predictive model:  

    * Data preparation for forecasting;
    * Feature engineering - encoding and scaling features, creating new ones, removing unnecessary ones;
    * Upsampling data;
    * Preparation for model creation.
    * Preliminary model training;
    * Hyperparameter tuning for the best models;
    * Model analysis, result validation on the test sample;
    * Checking the result for adequacy.  

### General Conclusion

In this work, we performed data preprocessing, exploratory data analysis, and created a model to predict whether a client will switch to competitors or not.

During the exploratory analysis, it was concluded that internet users with non-automatic monthly payments are more inclined to terminate collaboration with our company. This could be influenced by new competitors as well as problems with the form or payment algorithm on the site.

In the phase of creating the predictive model, we trained several different models, with the best result shown by the gradient boosting model from the sklearn library.

* AUC-ROC = 0.91,
* Accuracy score = 0.87
This result passed an adequacy check and is above the maximum target result set by the client.
