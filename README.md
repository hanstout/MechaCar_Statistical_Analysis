# MechaCar_Statistical_Analysis
## Linear Regression to Predict MPG (D1)
##### Steps: 
1. Download the MechaCar_mpg.csv file, and place it in the active directory for your R session.  
2. Create a new RScript in your R source pane, name it MechaCarChallenge.RScript, and save it to your active directory.
3. Use the library() function to load the dplyr package.
4. Import and read in the MechaCar_mpg.csv file as a dataframe.
5. Perform linear regression using the lm() function. In the lm() function, pass in all six variables (i.e., columns), and add the dataframe you created in Step 4 as the data parameter.
6. Using the summary() function, determine the p-value and the r-squared value for the linear regression model.
7. Save your MechaCarChallenge.RScript file to your GitHub repository.
##### Questions: 
* Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?  
The Vehicle Length and the Ground Clearance variables. This is due to low P-values, showing greater statistical significance when pretaining to mpg values in the dataset.
* Is the slope of the linear model considered to be zero? Why or why not?  
No, the slope is not considered to be zero. This is because the p-value is 5.35e-11 (below 0.05), all coefficents are not zero. The R-value is also closer to 1 than it is 0. See below image. 
* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?  
Yes, this model predicts the mpg of MechaCar prototypes is effective due to the adjusted R-squared being 0.6825. Meaning that 68.25% of variation is explained. 
<img src="Images/D1.PNG" width="400"/>

## Summary Statistics on Suspension Coils (D2)
##### Steps: 
1. Download the Suspension_Coil.csv file, and place it in the active directory for your R session.
2. In your MechaCarChallenge.RScript, import and read in the Suspension_Coil.csv file as a table.
3. Write an RScript that creates a total_summary dataframe using the summarize() function to get the mean, median, variance, and standard deviation of the suspension coil???s PSI column.
4. Write an RScript that creates a lot_summary dataframe using the group_by() and the summarize() functions to group each manufacturing lot by the mean, median, variance, and standard deviation of the suspension coil???s PSI column.
5. Save your MechaCarChallenge.RScript file to your GitHub repository.
##### Question: 
* The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?  
<img src="Images/D2.1.PNG" width="400"/>
Overall, when looking at the visuals provided, overall the data meet the 100 pound per square inch requirement. It is shown at about 62 variance. Taking a closer look at each lot provides more information. Both lots 1 and 2 meet the requirement of 100 pounds, but lot 3 does not. Lot 3 exceeds requirements greatly.  
<img src="Images/D2.2.PNG" width="400"/>

## T-Tests on Suspension Coils (D3)
##### Steps: 
1. In your MechaCarChallenge.RScript, write an RScript using the t.test() function to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.
2. Next, write three more RScripts in your MechaCarChallenge.RScript using the t.test() function and its subset() argument to determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 pounds per square inch.
3. Save your MechaCarChallenge.RScript file to your GitHub repository.

##### Findings: 
* Overall:  
<img src="Images/D3.0.PNG" width="400"/> 
The p-value is higher than the critical value of 0.05 and the mean is 1498.78, therefore failing to reject the hypothesis, with a 95% confidence range between 1497.5 and 1500 PSI.
* Lot 1:  
<img src="Images/D3.1.PNG" width="400"/>  
The p-value is higher than the critical value of 0.05 and the mean is exactly 1500 PSI, therefore failing to reject the hypothesis, with a 95% confidence range.
* Lot 2:  
<img src="Images/D3.2.PNG" width="400"/>   
The p-value is higher than the critical value of 0.05 and the mean is 1500.2, therefore failing to reject the hypothesis with a 95% confidence range between 1499.423 and 1500.977 PSI.
* Lot 3:  
<img src="Images/D3.3.PNG" width="400"/>  
The p-value is higher than the critical value of 0.05 and the mean is 1496.14, therefore rejecting the hypothesis as it does not meet the benchmark of 1500 pSI  with a 95% confidence range between 1492.431 and 1499.849 PSI.

## Study Design: MechaCar vs Competition (D4)  
A statistical study will compare the performance of MechaCar versus other vehicle manufactures on the market.  
Hypothesis: If an improved version of MechaCar is put up against other manufatcures, then their vehicles will have a higher saftey rating.  
Null Hypothesis: If the improved MechaCar version does not have a higher safety rating, then it will not have a higher safety rating than the competition.  
The statistical testing that could be used is a t-test. It can compare the means of safety ratings amoung groups of vehicles and determine the significant difference. In order to preform this test, data on safey ratings is needed from both MechaCar and other manufactures. It may be beneficial to include more than one other manufacturer if possible. 

