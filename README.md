# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
Please refer to the following figure for the linear regression analysis:

![Linear Regression Output](https://github.com/baumgartner-99/MechaCar_Statistical_Analysis/blob/main/images/Deliverable1_Output.png)

**Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?**

There were a couple coefficients who had low p-values, meaning that the amount of variance to the mpg values is non-random. Those coefficients are vehicle length and ground clearance.

**Is the slope of the linear model considered to be zero? Why or why not?**

The slope is not considered to be zero, since all of the coefficients have a value. If there was a zero slope, all of the coefficients would be nonexistent or extremely small. From the linear regression model, it is evident that there are at least two factors that have a linear relationship with mpg values.

**Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?**

I do not think this model predicts mpg of MechaCar prototypes effectively, because the ratio of statistically significant coefficients to coefficients in general is too small. Out of the 5 columns, there are only two that have a statistically significant impact on mpg values. That's not even half. Additionally, there could be other factors at play that are not shown in this model.

## Summary Statistics on Suspension Coils
For an analysis on summary statistics, please refer to the following images:

![Table 1](https://github.com/baumgartner-99/MechaCar_Statistical_Analysis/blob/main/images/Deliverable2_Total_Summary.png)

![Table 2](https://github.com/baumgartner-99/MechaCar_Statistical_Analysis/blob/main/images/Deliverable2_Lot_Summary.png)

Based on the manufacturing data, the variance of the suspension coils for all the manufacturing lots in total does not exceed 100 pounds per square inch. For all the lots in total, the variance is only 62.3 pounds per square inch. For each lot individually, Lot 1 and Lot 2 meet the design specifications with variance values under 10 pounds per square inch. The suspension coils in Lot 3 do exceed the limit with a variance of 170.3 pounds per square inch. 

## T-Tests on Suspension Coils
For information on T-Tests, please review the following screenshots and subsequent analysis:

![Full T-Test](https://github.com/baumgartner-99/MechaCar_Statistical_Analysis/blob/main/images/T-Test%20Sample%20PSI.png)

The results of this t-test are from a random sample of data from the Suspension Coil dataset. Because the p-value is larger than 0.05, we fail to reject the null hypothesis - that the mean of the sample set is not statistically different than the mean from the population set.

![T-Test Lot 1](https://github.com/baumgartner-99/MechaCar_Statistical_Analysis/blob/main/images/T-test-Lot1.png)

The results of this t-test are from a filtered subset of the population data: PSI values from Manufacturing Lot 1 only. The p-value here is less than 0.05 so we can reject the null hypothesis and conclude that the mean of this subset is statistically different than the mean from the population set.

![T-Test Lot 2](https://github.com/baumgartner-99/MechaCar_Statistical_Analysis/blob/main/images/T-test-Lot2.png)

The results of this t-test are from a filtered subset of the population data: PSI values from Manufacturing Lot 2 only. The p-value here is also less than 0.05 so we can reject the null hypothesis and conclude that the mean of this subset is statistically different than the mean from the population set.

![T-Test Lot 3](https://github.com/baumgartner-99/MechaCar_Statistical_Analysis/blob/main/images/T-test-Lot3.png)

The results of this t-test are from a filtered subset of the population data: PSI values from Manufacturing Lot 3 only. The p-value here is greater than 0.05 so we fail to reject the null hypothesis and can conclude that the mean of this subset is not statistically different from the population set.

## Study Design: MechaCar vs. Competition
A statistical study to quantify how the MechaCar performs against the competition could be a single linear regression looking at the monetary cost vs the maintenance cost so consumers can see how much their dollar is worth. Metrics to test would be the monetary price in US dollars that the car is sold for and maintenance costs for the following 5 years. The independent variable would be the amount sold for the car while the dependent variable would be to look at the maintenance costs. The null hypothesis would be that there is no relationship between car value and maintenance costs. The alternative hypothesis would be that there is a relationship between car value and maintenance costs. A linear regression test would be helpful to look at this so that users could identify the value of their dollar before purchasing the vehicle.
