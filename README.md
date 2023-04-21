# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

-   Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
	* The  **vehicle length**, and  **vehicle ground clearance**  are statistically likely to provide non-random amounts of variance to the model. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. The other variables have p-values that indicate a random amount of variance with the dataset.
    
-   Is the slope of the linear model considered to be zero? Why or why not?
    * The slope of the linear model is not considered to be zero because the p-value is 5.35e-11 which is significantly smaller than the significance level of 0.05%.
-   Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
	* This linear model has an r-squared value of 0.7149, which means that the model can predict mpg approximately 71% of the time.  Relatively speaking, the models prediction of mpg are effective.

![Linear Regression](https://github.com/BlazeMedina/MechaCar_Statistical_Analysis/blob/main/Images/Linear%20Regression.png)

## Summary Statistics on Suspension Coils

-  The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
	* The variance for the total lot specification is 62.29356. This does not exceed the 100 pounds per square inch requirement and therefore meets the manufacturing design specification. However, looking at the lots individually, not all lots meet the requirements. Both Lot 1 and Lot 2 variances are very much under the requirement. However, Lot 3 has a variance of 170.2861224, way above the requirement.  Manufacturing Lot 3 needs to be further inspected.
![Total Summary](https://github.com/BlazeMedina/MechaCar_Statistical_Analysis/blob/main/Images/total_summary.png)
![Lot Summary](https://github.com/BlazeMedina/MechaCar_Statistical_Analysis/blob/main/Images/lot_summary.png)

## T-Tests on Suspension Coils

From the results of the T-Test we can see the true mean of the sample is 1498.78. With a p-value of 0.06028, which is higher than the common significance level of 0.05, there is NOT enough evidence to support rejecting the null hypothesis. That is to say, the mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.
![Total T-Test](https://github.com/BlazeMedina/MechaCar_Statistical_Analysis/blob/main/Images/T%20Test.png)

1.  Lot 1 sample actually has the true sample mean of 1500. With a p-value of 1, clearly we cannot reject the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).
2.  Lot 2 sample has a sample mean of 1500.02, a p-value of 0.6072; the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.
3.  However, Lot 3, not surprisingly is a different scenario. Here the sample mean is 1496.14 and the p-Value is 0.04168, which is lower than the common significance level of 0.05. All indicating to reject the null hypothesis that this sample mean and the presumed population mean are not statistically different. Lot 3's production cycle must be checked for system failures
![Lots T-Test](https://github.com/BlazeMedina/MechaCar_Statistical_Analysis/blob/main/Images/lots_T_%20Test%20.png)

## Study Design: MechaCar vs Competition

To compare the performance of the MechaCar to other vehicles, we would need to collect many metrics including: cost, fuel efficiency, cost of ownership, vehicle category, number of seats, safety ratings.  If we were to explore the question of price, we could create a null hypothesis as follows: MechaCar is priced comparatively to vehicles with similar metrics.  The Alternative hypothesis would be: The MechaCar is not priced comparative to vehicles with similar metrics.  To test the hypothesis we would use multiple T-Tests to determine which factors influence price and how the MechaCar compares based on those factors.  The data for these tests would be determined from the first tests that determine which factors influence price.
