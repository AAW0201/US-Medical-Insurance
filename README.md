# US-Medical-Insurance
Analyzing BMI in relation to insurance charges

## Project Scope
### Questions:
* On average, do individuals with a BMI considered “underweight” have higher insurance costs than those with “healthy” or “overweight” BMIs?
* Which residential region has the highest average BMI?
* Which has the lowest?
* Do areas with higher BMIs also have higher insurance costs on average?
* Do smokers tend to have higher or lower BMI scores on average than non-smokers?

## Goals:
Determine whether higher or lower BMIs correlate to variances in insurance costs. 

## Data:
For this project, we’ll be using the medical insurance costs dataset provided by Codecademy. The dataset covers roughly 1,300 individuals with entries reflecting each individual’s age, biological sex, Body Mass Index (BMI), number of children, smoker status, residential region, and total charges paid by the insurance company. 

It is important to note that the dataset does not include any additional information such as other medical conditions or environmental factors that may lead to increased costs. It is also important to note that BMI is a quantitative measure and not necessarily an accurate predictor of health. Insurance companies use BMI in their calculations and so it features in this project.

For the purposes of this project, BMI classifications will be based on CDC classifications:

Less than 18.5 = Underweight
18.5 to < 25  = Healthy weight
25 to < 30 = Overweight
30 to < 35 = Obesity Class 1
35 to < 40 = Obesity Class 2
< 40 = Obesity Class 3 (Severe Obesity)

## Findings:
The average charge for customers with a BMI classified as Underweight is $8852.2.
The average charge for customers with a BMI classified as Healthy is $10434.53.
The average charge for customers with a BMI classified as Overweight is $10989.85.
The average charge for customers with a BMI classified as Obese Class 1 is $14429.42.
The average charge for customers with a BMI classified as Obese Class 2 is $17022.26.
The average charge for customers with a BMI classified as Obese Class 3 - Severe Obesity is $16440.51.

The Underweight class has the lowest average BMI at $8852.2.

The Obese Class 2 class has the lowest average BMI at $17022.26.

The Southwest, on average, is overweight with a BMI of 25.8.
The Southeast, on average, is obese (class 2) with a BMI of 36.85.
The Northwest, on average, is overweight with a BMI of 29.07.
The Northeast, on average, is obese (class 1) with a BMI of 31.92.

The Southeast has the highest average BMI at 36.85.

The Southwest has the lowest average BMI at 25.8.

The Southwest has an average charge of $2007.94.
The Southeast has an average charge of $1629.83.
The Northwest has an average charge of $29141.36.
The Northeast has an average charge of $2205.98.

The Northwest has the highest average charges with $29141.36.

The Southeast has the lowest average charges with $1629.83.

The Southwest has 58 smokers, with average charges of $32269.06 and an average BMI of 31.01, and 267 non-smokers with average charges of $8019.28 and an average BMI of 30.51. There's a 0.5 point difference in average BMI and a 120.38% difference in average charges between smokers and non-smokers. 21.72% of the customers in the region are smokers. 

The Southeast has 91 smokers, with average charges of $34845.0 and an average BMI of 33.1, and 273 non-smokers with average charges of $8032.22 and an average BMI of 33.44. There's a 0.3399999999999963 point difference in average BMI and a 125.07% difference in average charges between smokers and non-smokers. 33.33% of the customers in the region are smokers. 

The Northeast has 67 smokers, with average charges of $29673.54 and an average BMI of 28.57, and 257 non-smokers with average charges of $9165.53 and an average BMI of 29.33. There's a 0.759999999999998 point difference in average BMI and a 105.61% difference in average charges between smokers and non-smokers. 26.07% of the customers in the region are smokers. 

The Northwest has 58 smokers, with average charges of $30192.0 and an average BMI of 29.14, and 267 non-smokers with average charges of $8556.46 and an average BMI of 29.21. There's a 0.07000000000000028 point difference in average BMI and a 111.67% difference in average charges between smokers and non-smokers. 21.72% of the customers in the region are smokers. 



## Analysis:
If we look purely at the CDC categories on Body Mass Index we see a positive correlation between higher BMIs and higher insurance charges up until the “Obese Class 2” category, at which point we see the average charges begin to fall again. 

However, when we look at regions as a whole, we see that the Southeast region, which is classified as “obese (class 2)” has the highest average BMI and the lowest average of insurance charges while the highest average charges belong to the Northwest, a region considered “overweight.” 


Comparing smoker status reveals that smokers and non-smokers do not have a significant difference in average BMI; of the four regions within the data set, each had less than a one point difference in average BMI when comparing smokers and non-smokers. Smokers, however, do have significantly higher average insurance costs. In each of the four regions, the average charges for smokers were more than double the average charge of non-smokers. It is conceivable that an area with a high concentration of smokers may also show higher average insurance charges and skew the available data when only considering BMI information. However, the Southeast, which has the highest smoking percentage in its population, has the lowest average charges of the four regions.

At no point does the data reflect “severe obesity” having the most significant connection to higher insurance charges. 
