
## Modeling the Gold Ore Enrichment Process
### Toolkit
* Deep data preprocessing: merging multiple tables, filling in gaps, detecting outliers and anomalies;
* Creation of the SMAPE metric and its application in model validation;
* Visualization of initial data using matplotlib and seaborn libraries;
* Testing models with sklearn library.
### Input Data
A mining company is developing a model for predicting the quality of ore enrichment. The algorithm calculates the output of gold from raw material. The model allows input of only rich raw materials based on small samples.
### Objective
To create a model that predicts the content of precious metals and slag at various stages of enrichment.
### Project Structure
1. Data preparation.
    * Study of available files;
    * Checking the correctness of enrichment efficiency calculation;
    * Analysis of features not available in the test sample;
    * Data preprocessing and filling in gaps;
2. Data analysis.
    * Studying how the concentration of metals (Au, Ag, Pb) changes at various stages of purification;
    * Comparing the distribution of raw material grain sizes in the training and test samples;
    * Examining the total concentration of all substances at different stages: in raw materials, in rough and final concentrates.
3. Building a predictive model.
    * Creation of a function for calculating final sMAPE;
    * Training different models and evaluating their quality by cross-validation;
    * Selecting the best model and testing it on the test sample.
4. Conclusion.

### Общий вывод  
The goal of this project was to develop a model for predicting the sMAPE metric - the symmetric mean absolute percentage deviation.
In the third step, a Random Forest model was successfully created and is ready for implementation.

The tasks of the project were as follows:  

*Data Preparation:*  
At this stage, missing values were processed and unknown targets were removed for subsequent model building.

*Exploratory Data Analysis:*  
The following patterns were noted - the concentration of gold increases systematically at all stages of enrichment. The concentration of silver in the final concentrate is lower than in raw materials. The share of lead increases after primary purification, but then remains unchanged.
The overall concentration of metals in the solution shows a significant increase after flotation, however, it does not grow during subsequent purification.

*Building and Training the Model:*   
Four models were tested - regression, decision tree, random forest, and nearest neighbors.
The best model turned out to be the RandomForest model, which showed an sMAPE value of 5.99, which is an acceptable level for this project.
