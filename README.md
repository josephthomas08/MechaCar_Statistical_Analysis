# MechaCar_Statistical_Analysis
## Statistical Analysis using R

## Project Overview 
The MechaCar Project invloves use of Stats and Hypothesis testing to analyze sets of datasets from the automative industry 
The statistical analysis and visualizations is written in the R programming language.

## Resources
Data Source: MechaCar_mpg.csv, Suspension_Coil.csv
Software: RStudio
Version 1.4.1106

## Deliverable 1 


### D1.1 The MechaCar_mpg.csv file is imported and read into a dataframe 


<img width="645" alt="MODULE 15 D1 1" src="https://user-images.githubusercontent.com/75267605/114289925-98190a00-9a49-11eb-8b14-8137c259e1ad.png">


<img width="495" alt="Module 15 D1 1A" src="https://user-images.githubusercontent.com/75267605/114289927-9ea78180-9a49-11eb-8b3e-9f2f8b3c7b86.png">


### D1.2 An RScript is written for a linear regression model to be performed on all six variables 





<img width="897" alt="Module 15 D1 2" src="https://user-images.githubusercontent.com/75267605/114289943-bda61380-9a49-11eb-9b40-9b95ff25d8c7.png">





### D1.3 An RScript is written to create the statistical summary of the linear regression model with the intended p-values 


<img width="899" alt="Module 15 D1 3" src="https://user-images.githubusercontent.com/75267605/114289963-d9a9b500-9a49-11eb-99a1-7c0fdf2b24d6.png">

The summary o/p image, each Pr(>|t|) value represents the probability that each coefficient contributes a random amount of variance to the linear model. The results further emphasizes that vehicle length and ground clearance as well intercept extends a non-random amount of variance to the linear model of mpg. 



### D1.4 There is a summary that addresses all three questions

The above captured image from R analytical tool provides us with sufficent evidence that the probability values of the variables especially  "Vehicle Length" and "Ground Clearance" are very much smaller from our significant value of 0.05. These variables provide non random amount of variance to MPG values.

The p-value is 5.35e-11 which is much smaller than our assumed significance value of 0.05, hence we have sufficient evidence that slope of our linear model is not 0.

The r-squared value is 0.7 which as we understand predicts that  the future data points will fit to our linear model therefore  we can safely consider that this model effectively predcits the MPG of MechaCar prototypes.

Further R-square which .71 hence 71% of all the variations on mpg could be associated with the changes in the vehcile lenght, weight, drivetrain, spoiler angle and the ground clearance.






## Deliverable 2 


### D2.1 The Suspension_Coil.csv file is imported and read into a dataframe 


<img width="340" alt="Module 15 D2 1" src="https://user-images.githubusercontent.com/75267605/114290138-525d4100-9a4b-11eb-847c-a13e4aa36ddb.png">



<img width="605" alt="Module 15 D2 1A" src="https://user-images.githubusercontent.com/75267605/114290140-58532200-9a4b-11eb-8abc-a27e8ea2f96d.png">


### D2.2 An RScript is written to create a total summary dataframe that has the mean, median, variance, and standard deviation of the PSI for all manufacturing lots 

<img width="336" alt="Module 15 D2 2" src="https://user-images.githubusercontent.com/75267605/114290158-76208700-9a4b-11eb-9a43-7a4d1edcd922.png">


<img width="421" alt="Module 15 D2 2A" src="https://user-images.githubusercontent.com/75267605/114290163-7c166800-9a4b-11eb-8db3-c91644328c4b.png">



### D2.3 An RScript is written to create a lot summary dataframe that has the mean, median, variance, and standard deviation for each manufacturing lot 

<img width="496" alt="Module 15 D2 3" src="https://user-images.githubusercontent.com/75267605/114290178-95b7af80-9a4b-11eb-9f40-61fc0e53aa5b.png">


<img width="550" alt="Module 15 D2 3A" src="https://user-images.githubusercontent.com/75267605/114290185-9b14fa00-9a4b-11eb-8f3c-3ab24d4759ed.png">


### D2.4 There is a summary that addresses the design specification requirement for all the manufacturing lots and each lot individually 


The above detailed images  confirms that the variance of all manufacturing lots is 62.3 which is lower than the accepted level of 100, hence we safely confirm that overall it meets the design specification.

We can further confirm that it is the same case with lot 1 and lot 2 however  we see that the variance of lot 3 is 170 which is higher than the acceptable level. So we can state that the lot 1 and lot 2 meet the design specification but the lot 3 doesn't meet the specification level.

## Deliverable 3 

### T-Tests on Suspension Coils
We performed T-tests of whole data set and the three individual lots and as we see below are the screen shots of the results:

Sample T-Test of Whole Data


### D3.1 An RScript is written for t-test that compares all manufacturing lots against mean PSI of the population 


<img width="628" alt="Module 15 D3 1" src="https://user-images.githubusercontent.com/75267605/114290414-9c472680-9a4d-11eb-99cc-720e22e897b7.png">


##### Note : The key point  to watch out  in the above image  is the p-value of 0.06 which is higher than the assumed significance level of 0.05 therefore we dont have sufficient evidence to reject our null hypothesis and we would say that the two means are statistically similar.

### D3.2 An RScript is written for three t-tests that compare each manufacturing lot against mean PSI of the population 

#### Lot 1


<img width="802" alt="Module 15 D3 2A" src="https://user-images.githubusercontent.com/75267605/114290442-ce588880-9a4d-11eb-844b-72cc1a6aabc1.png">




#### Lot 2


<img width="815" alt="Module 15 D3 2B" src="https://user-images.githubusercontent.com/75267605/114290447-d7e1f080-9a4d-11eb-9cc4-ecf01d2f4388.png">




#### Lot 3



<img width="804" alt="Module 15 D3 2C" src="https://user-images.githubusercontent.com/75267605/114290451-dd3f3b00-9a4d-11eb-8a24-be0c5320fe8c.png">






### D3.3 There is a summary of the t-test results across all manufacturing lots and for each lot 

##### Note Lot 1:The p-value of Lot 1 is '1' which is higher than our assumed significance level of 0.05 hence we dont have sufficient evidence to reject our null hypothesis and we would state that the two means are statistically similar.


##### Note Lot 2:The p-value of Lot 2 is '0.6072' which is higher than our  assumed significance level of 0.05 hence  we dont have sufficient evidence to reject our null hypothesis and we would say that the two means are statistically similar.

##### Note Lot 3: The p-value of Lot 3 is '0.042' which is slightly lower thanour  assumed significance level of 0.05 therefore we would say that the two means are slightly different.





## Deliverable 4 


###  Design: MechaCar vs Competition
The study was conducted to quantify the performance of MechaCar against the competition, we will be studying the fuel consumption of the vehicles in the city area as  this is one of the most important factors for the city commuters. FOr this study, we will take the MPG (Miles Per Gallon) values in the city area of MechaCar and its competition.

Hence the metric to be tested is "MPG".

The other alternate hypothesis will be:

MechaCar will consume less fuel in its category of vehicles

We use the following statistical tests and the data:

The Fuel consumption of MechaCar and its competition at different driving conditions like at 10 mph , 50 mph and consumption at acceleration  will be done to check the MPG of each vehicle and then check the summary statistics to see Mean, Median and Std deviation.
Two sample T-test: We would specifically watch and record the p-value to check if there is any statistical difference between the means of two samples (MechaCar and Competition)


Alternative We can make a null hypothesis stating that it is not different from the competition and our Alternative would be the opposite. To engage  this we will additionaly need to use our t-test after collecting data from different types of competitor vehicles. Our t-test will be comparing the population of all types of competitor vehicles.

[link to MechCarChallenge.r file](https://github.com/josephthomas08/MechaCar_Statistical_Analysis/blob/main/MechaCarChallenge.R)

