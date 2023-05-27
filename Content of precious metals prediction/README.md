
## Modeling the process of gold ore enrichment
### Toolkit
Deep data preprocessing: combining multiple tables, filling in missing values, identifying outliers and anomalies.  
Creating the SMAPE metric and applying it in model validation.  
Visualization of the raw data using matplotlib and seaborn libraries.  
Testing models from the sklearn library.  
### Input data
A mining company is developing a model to predict the quality of ore enrichment. The algorithm calculates the gold yield from the raw material. The model can only accept rich ore based on small samples as input.
### Goal
Create a model that predicts the content of precious metals and slag at various stages of ore enrichment.
### Project structure  
1. Data Preparation.
   * Study the available files.
   * Verify the correctness of the enrichment efficiency calculation.
   * Analyze features that are not available in the test dataset.
   * Preprocess the data and fill in missing values.
2. Data Analysis.
   * Explore how the concentration of metals (Au, Ag, Pb) changes at different stages of purification.
   * Compare the particle size distribution of the feed material in the training and test datasets.
   * Investigate the total concentration of all substances at different stages: in the feed material, rougher and cleaner concentrates.
3. Building the Prediction Model.
   * Create a function to calculate the final sMAPE (symmetric mean absolute percentage error).
   * Train different models and evaluate their quality using cross-validation.
   * Select the best model and assess its performance on the test dataset.
4. Conclusion.

### Overall conclusion  
The goal of this project was to build a model for predicting the sMAPE (symmetric mean absolute percentage error) metric. In the third step, a Random Forest model was successfully developed and ready for deployment.

The project tasks included:

1. Data Preparation:
   * Handling missing values and removing rows with unknown targets to prepare the data for model building.
2. Data Analysis:
   * Discovering patterns such as the increasing concentration of gold at each stage of enrichment.
   * Observing that the concentration of silver in the final concentrate is lower than in the feed material.
   * Noting that the lead concentration increases after primary purification but remains stable afterward.
   * Analyzing the overall concentration of metals in the solution, which shows significant growth after flotation but remains relatively constant during subsequent purification stages.
3. Model Building and Training:
   * Testing four models: Regression, Decision Tree, Random Forest, and K-Nearest Neighbors.
   * Selecting the Random Forest model as the best performer, with an sMAPE value of 5.99, which meets the acceptable level for this project.    

In conclusion, the project successfully achieved the goal of building a model to predict the sMAPE metric. The Random Forest model demonstrated good performance and can be deployed for operational use.
