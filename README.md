# MechaCar_Statistical_Analysis
Module 15. Bootcamp


## Linear Regression to Predict MPG

### Data
![alt text](img/data.png)

These assumptions are taken to be true.

1. The input data is numerical and continuous.

2. The input data should follow a linear pattern.

3. There is variability in the independent x variable. This means that there must be more than one observation in the x-axis and they must be different values.

4. The residual error (the distance from each data point to the line) should be normally distributed.

### Problem
1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

        The Pr(>|t|), of the variables greater than 5%, indicates that these variables have a low level of statistical significance of a regression coefficient.

            - vehicle_weigth
            - spoiler_angle
            - AWD

2. Is the slope of the linear model considered to be zero? Why or why not?

        The p-value of the model is 5.35e-11, which is much lower than the assumed significance level of 0.05%. Therefore, the slope of the model is not zero.

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

        Yes, because the model has a multiple R-squared of 0.7149, which tells us that it is 71.49% that this model can be explained by the predictor variables

## Results
### Data analysis results
![alt text](img/dataAnalysis.png)

### Multilinear Regression plot
![alt text](img/mrlMerchaCar.png)

_________________________

## Summary Statistics on Suspension Coils

### Data
![alt text](img/datasus.png)

### Problem
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

## Results
### Statics analysis
The current manufacturing data meets the design specification if the total data is taken from the three manufacturing lot, with a variance value of 62.29 pounds per square inch.

But this calculation is wrong since it is averaged over 3 manufacturing lot. Two of them comply with the rule and one exceeds the limit with 170.28 pounds per square inch.

### Total summary
![alt text](img/totalsum.png)

### Manifacturing Lot summary
![alt text](img/lotsum.png)

_________________________
## T-Tests on Suspension Coils

The level of statistical significance is often expressed as a p-value between 0 and 1. The smaller the p-value, the stronger the evidence that you should reject the null hypothesis.

- A small p (≤ 0.05), reject the null hypothesis. This is strong evidence that the null hypothesis is invalid.
- A large p (> 0.05) means the alternate hypothesis is weak, so you do not reject the null.

For the population, the p-value is 0.06, this suggests there is NOT significant difference between the means of 1500 and the mean population. Not reject null hypothesis, the alternative hypothesis is weak.

### T-test Total Population
![alt text](img/ttesttotal.png)

For the sample Lot-1, the p-value is 1, Theres is no difference between the means.
### T-test Lot-1 Sample
![alt text](img/ttest1.png)

For the sample Lot-2, the p-value is 0.06, this suggests there is NOT significant difference between the means of 1500 and the sample mena. Not reject null hypothesis, the alternative hypothesis is weak.
### T-test Lot-2 Sample
![alt text](img/ttest2.png)

For the sample Lot-3, the p-value is 0.04, this suggests there is a significant diference between the means of the 1500. and the sample mean. Reject null hypothesis.
### T-test Lot-3 Sample
![alt text](img/ttest3.png)


_________________________

## Study Design: MechaCar vs Competition

1. Metrics to test
- Cost 
- City fuel efficiency
- Highway fuel efficiency 
- Useful life
- Type
- Model
- Cilinders
- Robberies


2. Null hypothesis 
- Truck fuel efficiency is positive related to cylinders and horsepower in city
- Car fuel efficiency is positive related to cylinders and horsepower in city
- Truck fuel efficiency is positive related to cylinders and horsepower in highway
- Car fuel efficiency is positive related to cylinders and horsepower in highway
- It's easier to steal an old truck than a new one
- It's easier to steal an old car than a new one


3. Alternative hypothesis
- Truck fuel efficiency is negative related to cylinders and horsepower in city
- Car fuel efficiency is negative related to cylinders and horsepower in city 
- Truck fuel efficiency is negative related to cylinders and horsepowerin highway
- Car fuel efficiency is negative related to cylinders and horsepower in highway
- It's not easier to steal an old truck than a new one
- It's not easier to steal an old car than a new one


4. Statistical test
- Two samples t-test
        For robberies info
- Simple linear regression 
        For efficiency fuel info
- Multiple linear regression
        For efficiency fuel info



5. What data is needed to run the statistical test?
This information from MecharCars and the competition, 3 years.
- Cost 
- City fuel efficiency
- Highway fuel efficiency 
- Useful life
- Type
- Model
- Cilinders
- Robberies 
