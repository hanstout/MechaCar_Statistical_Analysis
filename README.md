# MechaCar_Statistical_Analysis
## Linear Regression to Predict MPG (D1)
##### Steps: 
1. 
##### Questions: 
* Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?  
The Vehicle Length and the Ground Clearance variables. This is due to low P-values, showing greater statistical significance when pretaining to mpg values in the dataset.
* Is the slope of the linear model considered to be zero? Why or why not?  
No, the slope is not considered to be zero. This is because the p-value is 5.35e-11 (below 0.05), all coefficents are not zero. The R-value is also closer to 1 than it is 0. See below image. 
* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?  
Yes, this model predicts the mpg of MechaCar prototypes is effective due to the adjusted R-squared being 0.6825. Meaning that 68.25% of variation is explained. 
(IMAGE)

## Summary Statistics on Suspension Coils (D2)
##### Steps: 
1. 
##### Question: 
* The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?  
Overall, when looking at the visuals provided, overall the data meet the 100 pound per square inch requirement. It is shown at about 62 variance. Taking a closer look at each lot provides more information. Both lots 1 and 2 meet the requirement of 100 pounds, but lot 3 does not. Lot 3 exceeds requirements greatly. 
(IMAGES)

## T-Tests on Suspension Coils (D3)
##### Steps: 
1. 
##### Findings: 
* Overall:  
(Image)  
The p-value is higher than the critical value of 0.05 and the mean is 1498.78, therefore failing to reject the hypothesis, with a 95% confidence range between 1497.5 and 1500 PSI.
* Lot 1:  
(Image)  
The p-value is higher than the critical value of 0.05 and the mean is exactly 1500 PSI, therefore failing to reject the hypothesis, with a 95% confidence range.
* Lot 2:  
(Image)  
The p-value is higher than the critical value of 0.05 and the mean is 1500.2, therefore failing to reject the hypothesis with a 95% confidence range between 1499.423 and 1500.977 PSI.
* Lot 3:  
(Image)  
The p-value is higher than the critical value of 0.05 and the mean is 1496.14, therefore rejecting the hypothesis as it does not meet the benchmark of 1500 pSI  with a 95% confidence range between 1492.431 and 1499.849 PSI.

## Study Design: MechaCar vs Competition
