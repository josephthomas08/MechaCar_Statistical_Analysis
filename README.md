# MechaCar_Statistical_Analysis
Statistical Analysis using R


## Deliverable 1 


### D1.1 The MechaCar_mpg.csv file is imported and read into a dataframe 


<img width="645" alt="MODULE 15 D1 1" src="https://user-images.githubusercontent.com/75267605/114289925-98190a00-9a49-11eb-8b14-8137c259e1ad.png">


<img width="495" alt="Module 15 D1 1A" src="https://user-images.githubusercontent.com/75267605/114289927-9ea78180-9a49-11eb-8b3e-9f2f8b3c7b86.png">


### D1.2 An RScript is written for a linear regression model to be performed on all six variables 





<img width="897" alt="Module 15 D1 2" src="https://user-images.githubusercontent.com/75267605/114289943-bda61380-9a49-11eb-9b40-9b95ff25d8c7.png">





### D1.3 An RScript is written to create the statistical summary of the linear regression model with the intended p-values 


<img width="899" alt="Module 15 D1 3" src="https://user-images.githubusercontent.com/75267605/114289963-d9a9b500-9a49-11eb-99a1-7c0fdf2b24d6.png">


### D1.4 There is a summary that addresses all three questions

The above captured image from R analytical tool provides us with sufficent evidence that the probability values of the variables especially  "Vehicle Length" and "Ground Clearance" are very much smaller from our significant value of 0.05. These variables provide non random amount of variance to MPG values.

The p-value is 5.35e-11 which is much smaller than our assumed significance value of 0.05, hence we have sufficient evidence that slope of our linear model is not 0.

The r-squared value is 0.7 which as we understand predicts that  the future data points will fit to our linear model therefore  we can safely consider that this model effectively predcits the MPG of MechaCar prototypes.





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


The key point  to watch out  in the above image  is the p-value of 0.06 which is higher than the assumed significance level of 0.05 therefore we dont have sufficient evidence to reject our null hypothesis and we would say that the two means are statistically similar.

### D3.2 An RScript is written for three t-tests that compare each manufacturing lot against mean PSI of the population 

#### Lot 1

<img width="802" alt="Module 15 D3 2A" src="https://user-images.githubusercontent.com/75267605/114290442-ce588880-9a4d-11eb-844b-72cc1a6aabc1.png">

#### Lot 2
<img width="815" alt="Module 15 D3 2B" src="https://user-images.githubusercontent.com/75267605/114290447-d7e1f080-9a4d-11eb-9cc4-ecf01d2f4388.png">


#### Lot 3
<img width="804" alt="Module 15 D3 2C" src="https://user-images.githubusercontent.com/75267605/114290451-dd3f3b00-9a4d-11eb-8a24-be0c5320fe8c.png">


### D3.3 There is a summary of the t-test results across all manufacturing lots and for each lot 



## Deliverable 4 

### 4.1 A metric to be tested is mentioned 
### 4.2 A null hypothesis or an alternative hypothesis is described 
### 4.3 A statistical test is described to test the hypothesis
### 4.4 The data for the statistical test is described 
