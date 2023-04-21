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

Total Summary<br>
![Total Summary](https://github.com/BlazeMedina/MechaCar_Statistical_Analysis/blob/main/Images/total_summary.png)

Lot Summary<br>
![Lot Summary](https://github.com/BlazeMedina/MechaCar_Statistical_Analysis/blob/main/Images/lot_summary.png)
