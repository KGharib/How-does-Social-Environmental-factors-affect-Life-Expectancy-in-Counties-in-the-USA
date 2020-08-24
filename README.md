# How-does-Social-Environmental-factors-affect-Life-Expectancy-in-Counties-in-the-USA
## Introduction
I am part of a Consulting Group that have been asked to Analyze the Dataset and peform models

## Objectives

* Analyze and perform EDA on the Dataset
* Mainly Focusing on Using Linear Regression and continually fine tune them


### Final Project Summary
the Robert Wood Johnson Foundation and the University of Wisconsin
Population Health Institute have collected the Data and I am seeking to help them
save money, time and effort by refining and improving on their questionere and method of collecting data

**_Findings_**
After analyzing and cleaning the data I found that the main contributers to Years of Potential Life lost Rate(sum of difference between age of death and average age of death, in other words this would be the total of all the peoples difference between their age and the average age of death in the USA) for each county was most affected by these features:
* '%_LBW'
* '%_Obese'
* 'Food_Environment_Index'
* '%_Physically_Inactive'
* '%_With_Access'
* '%_Excessive_Drinking'
*  'Chlamydia_Rate'
*  'Teen_Birth_Rate'
*  'MHP_Rate'
*  'Preventable_Hosp_Rate'
*  'Graduation_Rate'
*  'Income_Ratio'
*  '%_Single_Parent_Households'
*  'Injury_Death_Rate'
*  'Average_Daily_PM25'
*  '%_Drive_Alone'
*  '%_Long_Commute___Drives_Alone'

we reduced the number of variables from 35 down to 16, we did this by firstly looking at Interactions, Multicollinearity and removed those variables that were highly correlated to each other. we also checked for Normality and Homoscedasticity and removed those outliers to ensure that the residuals were normalized and Homoscedastistic

Overall I found that these factors contributed most directly to Years of Potential Life lost Rate.
<br>
I then performed a normal Linear Regression Model a Ridge Regression Model and a Lasso Regression Model and we saw that our R2 for Ridge Regression models performed better then both our Lasso and Linear Regression Model. As our Ridge Regression Model performed better we decided to move forward with a Ridge Regression Model and used it to test our testing sample and our Model performed well with an R2 of 0.821

# Futher Works
Overall the main objective was to predict Years of Potential Life lost Rate based on certain features, the focus was to use all my Linear Regression knowledge to achieve this, for further works I would like to also implement KNN model as it would be a good fit for the dataset.
