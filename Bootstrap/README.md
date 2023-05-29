
## Analysis of Potential Profit and Risks of Oil Production in a Region
### Toolkit
Applying the bootstrap technique;  
Working with business metrics: gross, operating, net profit, conversions, online and offline indicators;  
Seaborn visualization.  
### Introduction
This project is being carried out for an extraction company that needs to decide where to drill a new well.  
Data on oil samples in three regions are provided: in each, 10,000 deposits were measured for oil quality and volume of its reserves.  
A machine learning model must be built that will help determine the region where extraction will bring the most profit.  
### Objective

To choose the most profitable region with a minimal risk of error.

### Project Structure

1. Loading and preparing data.
2. Training and testing on a validation sample model for each region. We will use the RMSE metric.
3. Creation of a function for calculating profit.
4. Applying Bootstrap to calculate risks and profit for each region.
5. Choosing a region for field development.

### Overall Conclusion

In this project, an analysis of oil fields in three regions was carried out to select the most promising one.  
The following actions were taken:

* Primary data processing was carried out;
* A primary analysis of each region was carried out, the correlations of features with the target and the distributions of the target feature were studied.
    * Regions 0 and 2 are similar to each other - they have a normal distribution of deposit volumes and similar feature correlations.
    * Region 1 has a 100% correlation of one feature with the target. The volume distribution is not normal;
* Linear regression models were trained and predictions of the volume of deposits in each region were made.
    * The best prediction result was obtained in Region 1 - the root mean square deviation is less than 1,000 barrels.
    * In Regions 0 and 2, the deviation is equal to 37 and 40 thousand barrels, but the average values of the entire sample are predicted accurately;
* In Regions 0 and 2, the deviation is equal to 37 and 40 thousand barrels, but the average values of the entire sample are predicted accurately;
* The Bootstrap technique with 1000 samples was used to find the average profit, 95% confidence interval, and risk of losses.
    * There is no risk of losses at the current price level in any of the regions.
    * By average profit values and confidence interval, the most profitable region is Region_1.
