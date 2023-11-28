![Movie Analysis Banner](images/movie_analysis_banner.jpg)
# House sales in a northwestern county

**Author**: Bijal Saija

## Overview

This data science project aims to address a critical business problem for our stakeholders, a real estate agency specializing in helping homeowners buy and sell homes. The primary focus is on providing valuable insights and advice to homeowners regarding how home renovations may impact the estimated value of their properties. I have used regression modeling to analyze house sales in a northwestern county for this project.
## Business Problem

The key business problem identified is the need to empower homeowners with actionable information about potential home renovations. The goal is to guide them in making informed decisions that can enhance the market value of their homes. By understanding the potential impact of specific renovations on the estimated property value, homeowners can prioritize and plan renovations strategically.

***

## Data

This project uses the King County House Sales dataset, which can be found in kc_house_data.csv
As with most real-world data sets, the column names were not perfectly described, so have done some research and I have used only those columns that affect house prices. 

So after deciding what feature from the dataset to use and how to use it. The selected features are as below:
price
bedrooms
bathrooms
sqft_living
sqft_lot 
floors
condition
grade
yr_built

Checking the information on the new data, I then dropped the unwanted data like id. This dataset will serve as the foundation for training and evaluating the predictive model.
***

## Methods

The project follows a data science lifecycle, encompassing data exploration, preprocessing, model development, and evaluation. The choice of algorithms, feature engineering techniques, and evaluation metrics will be explained in detail.

***
After checking the plot of each column there were so many outliers, that I decided to remove them as they can misguide the model to work properly. 

Developed a predictive model that estimates the impact of different types of home renovations on the overall value of a property.
Identified and analyzed relevant features within the dataset that significantly contribute to the estimated property value.
Created a recommendation system that suggests the most beneficial renovations based on the unique characteristics of each home.
***

## Results

Predictive Model: A machine learning model capable of estimating the impact of home renovations on property value.

Recommendation System: A system that provides personalized recommendations for home renovations based on the dataset analysis.

Documentation: Comprehensive documentation detailing the methodology, code structure, and explanations of key decisions made during the project.


***

***



## Conclusions

This analysis leads to three features that can lead to price rise:-

Checked for multicollinearity and had to remove if there was any in between two independent variables but there was not more than 0.7.

R-squared: 0.508
This indicates the proportion of the variance in the dependent variable (price) that is predictable from the independent variables. In this case, approximately 50.8% of the variability in the home prices is explained by the model.
Adjusted R-squared: 0.508
Similar to R-squared but adjusted for the number of predictors in the model. It provides a more accurate measure in the presence of multiple predictors.
Observations: 13,604

Degrees of Freedom (Df):

Residuals: 13,595
Model: 8
Total: 13,603
F-statistic: 1757.0

A measure of how well the overall model fits the data. A higher F-statistic suggests a better fit.
Prob (F-statistic): 0.00

The p-value is associated with the F-statistic. A low p-value indicates that the model is statistically significant.
Coefficients:
Intercept (const): 4.558e+05
Coefficients for Predictors:
sqft_living, sqft_lot, bedrooms, bathrooms, floors, grade, condition, yr_built
Each coefficient represents the change in the dependent variable (price) per one-unit change in the respective independent variable, holding other variables constant.
Statistical Significance:
t-statistic and P>|t|:
Indicates the statistical significance of each coefficient. The lower the p-value, the more significant the predictor. In this case, all predictors seem to be statistically significant (p-value < 0.05).
Model Fit:
AIC (Akaike Information Criterion): 3.6e+05
BIC (Bayesian Information Criterion): 3.601e+05
Information criteria that penalize models for complexity. Lower values indicate a better fit.
Residuals:
Omnibus: 721.155
Durbin-Watson: 2.008
Jarque-Bera (JB): 1023.301
Tests for normality and autocorrelation of residuals. A low Durbin-Watson suggests potential autocorrelation.
Notes:
Standard Errors: Assume that the covariance matrix of the errors is correctly specified.
This summary provides a comprehensive overview of the linear regression model, its fit to the data, and the statistical significance of each predictor. It suggests that the model explains a substantial portion of the variance in home prices, and the included predictors are statistically significant.

Questions to consider:

Further analysis may include checking for model assumptions and exploring the residuals in more detail.
***





## Repository Structure

Describe the structure of your repository and its contents, for example:

```
├── README.md                           <- The top-level README for reviewers of this project
├── microsoft_movie_analysis.ipynb      <- Narrative documentation of analysis in Jupyter notebook
├── microsoft_movie_analysis.pdf        <- PDF version of project presentation
├── zippedData                          <- Data repositories sourced externally
└── images                              <- Both sourced externally and generated from code
```
