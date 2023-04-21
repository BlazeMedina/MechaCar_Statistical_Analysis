# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

-   Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
	* The  **vehicle length**, and  **vehicle ground clearance**  are statistically likely to provide non-random amounts of variance to the model. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. The other variables have p-values that indicate a random amount of variance with the dataset.
    
-   Is the slope of the linear model considered to be zero? Why or why not?
    * The slope of the linear model is not considered to be zero because the p-value is 5.35e-11 which is significantly smaller than the significance level of 0.05%.
-   Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
	* This linear model has an r-squared value of 0.7149, which means that the model can predict mpg approximately 71% of the time.  Relatively speaking, the models prediction of mpg are effective.

![Linear Regression](https://github.com/BlazeMedina/MechaCar_Statistical_Analysis/blob/main/Images/Linear%20Regression.png)
