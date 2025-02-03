# US-Medical-Insurance
Analyzing BMI in relation to insurance charges

## Project Scope
### Questions:
On average, do individuals with a BMI considered “underweight” have higher insurance costs than those with “healthy” or “overweight” BMIs?
Which residential region has the highest average BMI?
Which has the lowest?
Do areas with higher BMIs also have higher insurance costs on average?
Do smokers tend to have higher or lower BMI scores on average than non-smokers?

##Goals:
Determine whether higher or lower BMIs correlate to variances in insurance costs. 
Data:
For this project, we’ll be using the medical insurance costs dataset provided by Codecademy. The dataset covers roughly 1,300 individuals with entries reflecting each individual’s age, biological sex, Body Mass Index (BMI), number of children, smoker status, residential region, and total charges paid by the insurance company. 

It is important to note that the dataset does not include any additional information such as other medical conditions or environmental factors that may lead to increased costs. It is also important to note that BMI is a quantitative measure and not necessarily an accurate predictor of health. Insurance companies use BMI in their calculations and so it features in this project.

For the purposes of this project, BMI classifications will be based on CDC classifications:
Less than 18.5 = Underweight
18.5 to < 25  = Healthy weight
25 to < 30 = Overweight
30 to < 35 = Obesity Class 1
35 to < 40 = Obesity Class 2
< 40 = Obesity Class 3 (Severe Obesity)


## Analysis:
If we look purely at the CDC categories on Body Mass Index we see a positive correlation between higher BMIs and higher insurance charges up until the “Obese Class 2” category, at which point we see the average charges begin to fall again. 

However, when we look at regions as a whole, we see that the Southeast region, which is classified as “obese (class 2)” has the highest average BMI and the lowest average of insurance charges while the highest average charges belong to the Northwest, a region considered “overweight.” 


Comparing smoker status reveals that smokers and non-smokers do not have a significant difference in average BMI; of the four regions within the data set, each had less than a one point difference in average BMI when comparing smokers and non-smokers. Smokers, however, do have significantly higher average insurance costs. In each of the four regions, the average charges for smokers were more than double the average charge of non-smokers. It is conceivable that an area with a high concentration of smokers may also show higher average insurance charges and skew the available data when only considering BMI information. However, the Southeast, which has the highest smoking percentage in its population, has the lowest average charges of the four regions.

At no point does the data reflect “severe obesity” having the most significant connection to higher insurance charges. 
