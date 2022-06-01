# MechaCar_Statistical_Analysis

# Overview of R Statistics 
Load, clean up, and reshape datasets using tidyverse in R. Visualize datasets with basic plots such as line, bar, and scatter plots using ggplot2. Generate and interpret more complex plots such as boxplots and heatmaps using ggplot2.
Plot and identify distribution characteristics of a given dataset. Formulate null and alternative hypothesis tests for a given data problem. Implement and evaluate simple linear regression and multiple linear regression models for a given dataset. Implement and evaluate the one-sample t-Tests, two-sample t-Tests, and analysis of variance (ANOVA) models for a given dataset. Implement and evaluate a chi-squared test for a given dataset. Identify key characteristics of A/B and A/A testing. Determine the most appropriate statistical test for a given hypothesis and dataset.

## Linear Regression to Predict MPG
* RScript was written for a linear regression model to be performed on all six variables 
![linear regression](https://user-images.githubusercontent.com/96156893/171408373-8483abb3-12c2-4e94-b8ff-26363a2d7266.png)

### Summary of Linear Regression model
* An RScript was written to create the statistical summary of the linear regression model with the intended p-values and the r-squared value
![Mechacar summary](https://user-images.githubusercontent.com/96156893/171408657-385edfd6-8a05-44c9-b54a-7e88931a6ed8.png)


#### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
* The R-squared value shows that the variations in the data can be explained by the model.The p-value is also significant, as it shows 5.35e-11. The vehicle's ground clearance and lenght are statistically significant.Furthermore, this gives the conclusion that the ground clearance and vehicle length displays non-random amounts of variances.

#### Is the slope of the linear model considered to be zero? Why or why not?
* The p-values values 5.35e-11vsupports the idea that there is strong relationship between the model and the variables. The slopes may appear to be close to zero but they are non-zero. 

#### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
* After running the analysis R-squared is .7149 which shows the dataset is effective. This linear model effectively predicts mpg of MechaCar prototypes. Although, roughly 71% will be determined by this model there may be other variable we are not coonsidering that can contribute to the mpg.

# Summary Statistics on Suspension Coils

 ### Total Summary
 * The mean, median, variance, and standard deviation of the suspension coil’s PSI column.
![total summary](https://user-images.githubusercontent.com/96156893/171408797-d789682c-e6f8-41b5-b07b-bfbc58dcb437.png)


 ### Lot Summary
 * Each manufacturing lot by the mean, median, variance, and standard deviation of the suspension coil’s PSI column.
![lot_summary](https://user-images.githubusercontent.com/96156893/171408805-daa6d1df-5104-499c-866f-7640266150ef.png)

### Analysis: 
* The designs specifications for the MechaCar suspension coils states the variance of the suspension coils must not exceed 100 pounds per square inch. The variance for the total manufacturing lot is 62 which does not exceeds the designs specifications. When we review the lots separately the results demonstrate Lot 1 and Lot 2 meet the 100 PSI variance requirement. However, Lot 3 does not meet the design specifications displaying a variance of 170.

# T-Tests on Suspension Coils
### T-test for Total Summary
* An RScript was written for t-test that compares all manufacturing lots against mean PSI of the population 

![All_lots_SC](https://user-images.githubusercontent.com/96156893/171408943-1c5d722e-a244-480e-b880-690d5fffb297.png)

* An RScript is written for three t-tests that compare each manufacturing lot against mean PSI of the population 
### T-test for Lot 1
![lot1](https://user-images.githubusercontent.com/96156893/171408841-c8c639f8-6772-4c97-83c4-3e9aee4eeb06.png)

### T-test for Lot 2
![lot2](https://user-images.githubusercontent.com/96156893/171408854-9c1b0bce-deda-42ed-822c-a569cb48c39e.png)

### T-test for Lot 3
![lot3](https://user-images.githubusercontent.com/96156893/171408872-2dc464f2-0e7c-4845-8b7d-36850a542ccc.png)

#### The T-test
* Lot 1 and Lot 2 show normal distribution there is not enough evidence to reject the null hypothesis. Lot 3 null hypothesis is rejected due to it exceeding the specification requirements. 

## Study Design: MechaCar vs Competition
* The next metrics to test should focus on the horsepower, highway fuel efficiency and saftey rating. These are few concerns the consumers have mentioned. The null hypothesis is that the safety rating is zero. The alternative hypothesis is that the safety rating is not zero.  I believe a Using a multiple linear regression statistical summary would be the best option.
