# Module 15 | MechaCar Manufacturing

## Overview
The purpose of this analysis is to offer insights on the MechaCar's production to help the manufacturing process. In order to conduct this analysis, we used programming language R and its dplyr library.

## Linear Regression to Predict MPG
 We designed a **multiple linear regression model** in order to predict the miles per gallon (mpg) dependent variable by using different variables from our dataset.
 First of all we need to define our hypothesis and answer the next questions:

- **Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?**
    - The "vehicle length" and the "ground_clearance". Both with small p-value so they had a high level of significance.
- **Is the slope of the linear model considered to be zero?**
    - NO, the linear regression shows that some of the independent variables had a significant effect on the dependent variable.
- Does this linear model predict mpg of MechaCar prototypes effectively?
    - The r-squared value is 0.7149 mean this means that out of 100 instances, this model would approximately predict the mpg of the MechaCar correctly 71 times.
![Linear_regression](https://github.com/davescudero/MechaCar_Statistical_Analysis/blob/main/Resources/Linear_regression.png)

## Summary Statistics on Suspensions Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch.
- **Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually?**
    - The variance for all manufacturing lots in total is 62.29, so this matches the specifications before. 
    - However, the lots separately, Lot3 is surpassing the 100 pounds per square inch criteria, with 170.28 PSI.
![Summary_Statistics_2](https://github.com/davescudero/MechaCar_Statistical_Analysis/blob/main/Resources/Summary_Statistics_2.png)
![Summary_Statistcis_1](https://github.com/davescudero/MechaCar_Statistical_Analysis/blob/main/Resources/Summary_Statistics_1.png)

## T-Tests on Suspension Coils
By perfroming the next analysis we wanted to realize if any of the four groups of Lots (lot1, lot2, lot3, and total lots) have a statistically different mean value from the population one (1,500 PSI)


all four p-values where much greater than .05 meaning that our  hypothesis fail to reject that there is a statistical difference between the four groups and the population mean.

Total lots t-test:
![Alllots_ttest](https://github.com/davescudero/MechaCar_Statistical_Analysis/blob/main/Resources/Alllots_ttest.png)
Lot 1 t-test:
![Lot1_ttest](https://github.com/davescudero/MechaCar_Statistical_Analysis/blob/main/Resources/Lot1_ttest.png)
Lot 2 t-test:
![Lot2_ttest](https://github.com/davescudero/MechaCar_Statistical_Analysis/blob/main/Resources/Lot2_ttest.png)
Lot 3 t-test:
![Lot3_ttest](https://github.com/davescudero/MechaCar_Statistical_Analysis/blob/main/Resources/Lot3_ttest.png)

## Study Design: MechaCar vs Competition

In order to know how well MechaCar performs against the competition we need to adress the following questions:

- **What metric or metrics are you going to test?**
    - I would test the metrics of city and highway fuel efficiencies.
- **What is the null hypothesis or alternative hypothesis?**
    - Null Hypothesi: All of the cars in the same class have the same fuel efficiency 
    - Alternative Hypothesis: is that they are not all the same.
- **What statistical test would you use to test the hypothesis?**
    - I think ANOVA test would be the best fit for this analysis, cause we can see if there´s any diference in the variance of the groups and present my results with a boxplot.
- What data is needed to run the statistical test?
    - I would need the fuel efficiency data for each type of car in order to collect the most information possible to do this analysis.




