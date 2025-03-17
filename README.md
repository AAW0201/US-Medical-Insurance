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
                   classification   charges
0                     underweight   8852.20
1                         healthy  10434.53
2                      overweight  10989.85
3                   obese class 1  14429.42
4  obese class 3 (severely obese)  16440.51
5                   obese class 2  17022.26

The Underweight class has the lowest average charges at $8852.20.

The Obese Class 2 class has the highest average charges at $17022.26.


      region        bmi classification
0  northeast  29.173503     overweight
1  northwest  29.199785     overweight
2  southwest  30.596615  obese class 1
3  southeast  33.355989  obese class 1

The northeast region has the lowest average bmi at 29.173503086419753, with an average classification of "overweight"

The southeast region has the highest average bmi at 33.35598901098901, with an average classification of "obese class 1"

    
    region   charges
  southwest  12346.94
  northwest  12417.58
  northeast  13406.38
  southeast  14735.41

The southwest region has the lowest average charges with $12346.94

The southeast region has the highest average charges with $14735.41


    region    smoker   charges      bmi   classification
  northeast   False   9165.53  29.332082     overweight
  northeast    True  29673.54  28.565224     overweight
  northwest   False   8556.46  29.212678     overweight
  northwest    True  30192.00  29.140431     overweight
  southeast   False   8032.22  33.442418  obese class 1
  southeast    True  34845.00  33.096703  obese class 1
  southwest   False   8019.28  30.507865  obese class 1
  southwest    True  32269.06  31.005172  obese class 1


The Northeast has 67 smokers, with average charges of $29673.54 and an average BMI of 28.565223880597014. The same region has 257 non-smokers with average charges of $9165.53 and an average BMI of 29.33208171206226. There's a 0.766857831465245 point difference in average BMI and a 223.75% difference in average charges between smokers and non-smokers. 20.68% of the customers in the region are smokers.

The Northwest has 58 smokers, with average charges of $30192.0 and an average BMI of 29.14043103448276. The same region has 267 non-smokers with average charges of $8556.46 and an average BMI of 29.21267790262172. There's a 0.07224686813896142 point difference in average BMI and a 252.86% difference in average charges between smokers and non-smokers. 17.85% of the customers in the region are smokers.

The Southeast has 91 smokers, with average charges of $34845.0 and an average BMI of 28.565223880597014. The same region has 273 non-smokers with average charges of $8032.22 and an average BMI of 33.44241758241758. There's a 0.345714285714287 point difference in average BMI and a 333.82% difference in average charges between smokers and non-smokers. 25.0% of the customers in the region are smokers.

The Southwest has 58 smokers, with average charges of $32269.06 and an average BMI of 31.005172413793108. The same region has 267 non-smokers with average charges of $8019.28 and an average BMI of 30.50786516853933. There's a 0.49730724525377923 point difference in average BMI and a 302.39% difference in average charges between smokers and non-smokers. 17.85% of the customers in the region are smokers.



## Analysis:
If we look purely at the CDC categories on Body Mass Index we see a positive correlation between higher BMIs and higher insurance charges up until the “Obese Class 2” category, at which point we see the average charges begin to fall again. 

When we look at regions as a whole, we see that the Southeast, which has the highest BMI at 33.355989, also has the highest average charges at $14735.41. However, the Northeast region, which has the lowest average BMI at 29.173503, has the second highest average charges at $13406.38. 

Comparing smoker status reveals that, while smokers in most regions do tend to have a slightly lower BMI than non-smokers, smokers and non-smokers do not have a significant difference in average BMI; of the four regions within the data set, each had less than a one point difference in average BMI when comparing smokers and non-smokers. Smokers, however, do have significantly higher average insurance costs. In each of the four regions, the average charges for smokers were more than double the average charge of non-smokers and regions with higher populations of smokers consistently have higher average insurance costs.  It is conceivable that an area with a high concentration of smokers may also show higher average insurance charges and skew the available data when only considering BMI information, as we see in the Northeast, which ranks lowest in average BMI, but second highest both in smoking population and average insurance costs. 

At no point does the data reflect “severe obesity” having the most significant connection to higher insurance charges. 
