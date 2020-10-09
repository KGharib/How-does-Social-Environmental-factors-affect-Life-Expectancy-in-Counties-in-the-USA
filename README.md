# How-does-Social-Environmental-factors-affect-Life-Expectancy-in-Counties-in-the-USA
## Introduction
I have bee asked as part of a Consulting Group to Analyze the Dataset and peform Machine Learning models in order to see how certain social environmental factors affect the life expectancy in different counties in the USA

## Objectives
* Analyze/perform EDA on the Dataset
* Cleaning and removing of messy data 
* Mainly Focusing on Using Linear Regression and continually fine tuning the model in order to predict which factors affect life expectancy the most

### Final Project Summary
the Robert Wood Johnson Foundation and the University of Wisconsin Population Health Institute have collected the Data and I am seeking to help them
save money, time and effort by refining and improving on their questionere and method of collecting data

**_Findings_**
After analyzing and cleaning we can see the main contributers to Years of Potential Life lost Rate(sum of difference between age of death and average age of death, in other words this would be the total of all the peoples difference between their age and the average age of death in the USA which is related to life expectancy, is expected age of death higher or lower than the average in the USA) for each county was most affected by these features:

* '%_LBW' - Percentage of births with low birth weight (<2500g)
* '%_Obese' - Percentage of adults that report BMI >= 30
* 'Food_Environment_Index' - Indicator of access to healthy foods 
* '%_Physically_Inactive' - Percentage of adults that report no leisure-time physical activity
*  %_Children_in_Poverty -Percentage of children (under age 18) living in poverty
* '%_Excessive_Drinking' - Percentage of adults that report excessive drinking
*  'Chlamydia_Rate' - Number of chlamydia cases
*  'Teen_Birth_Rate' - Births per 1,000 females ages 15-19
*  'Graduation_Rate' - Number of students expected to graduate
*  'Income_Ratio' - Ratio of household income at the 80th percentile to income at the 20th percentile
*  '%_Single_Parent_Households' - Number of children that live in single-parent households
*  'Injury_Death_Rate' - Injury mortality rate per 100,000
*  'Average_Daily_PM25' - Average daily amount of fine particulate matter in micrograms per cubic meter
*  '%_Drive_Alone' - Percentage of workers who drive alone to work
*  '%_Long_Commute___Drives_Alone' - Among workers who commute in their car alone, the percentage that commute more than 30 minutes

The number of variables was reduced from 35 to 15, this was done by looking at Interactions, Multicollinearity and removing those variables that were highly correlated to each other. Furthermore I checked for Normality and Homoscedasticity and removed those outliers to ensure that the residuals were normalized and Homoscedastistic

Overall I found that these factors contributed most directly to Years of Potential Life lost Rate.
<br>
I then performed a normal Linear Regression Model a Ridge Regression Model and a Lasso Regression Model. The R2 for both the Lasso and Ridge Regression models performed better then the Linear Regression Model. As both our Lasso and Ridge performed very similarly with an R2 of 0.826 I chose to move forward with a Ridge Regression Model and used it to test our testing sample and our Model performed well with an R2 of 0.821

# Futher Works
Overall the main objective was to predict Years of Potential Life lost Rate based on certain features, the focus was to use all my Linear Regression knowledge and skills to achieve this, for further works I would like to also implement KNN model as i feel it would be a good fit for the dataset.
