# BoomBike_Sharing_Assignment
> Case Study of Linear Regression model for a US bike-sharing provider BoomBikes.


## Table of Contents :
* [Problem Statement]
* [Objectives]
* [Approach]
* [Technologies Used]
* [Conclusions]
* [Acknowledgements]
* [Glossary]
* [Author]


## Problem Statement
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:
- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands.

Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors. 
 
 ## Objectives
You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 
Please find the [Bike Sharing dataset](./day.csv) and [Data dictionary](./Data%20dictionary.txt).

## Approach

- Step 1: Reading and Understanding the Data (BoomBike dataset)
--Import Necessary Libraries
--Analyzing the dataset
--Data Quality check
--Data Cleaning
- Step 2: Visualising the Data
- Step 3: Data Preparation
- Step 4: Splitting the Data into Training and Testing Sets
- Step 5: Rescaling the Features
--Dividing into X and Y sets for the model building
- Step 6: Building a linear model
--Checking VIF for multicollinearity
- Step 7: Residual Analysis of the train data
--Checking Error Terms and how the error has split
--Cross-verifying the above conclusion using a qq-plot as well
- Step 8: Making Predictions Using the Final Model
- Step 9: Model Evaluation
- Step 10: Making final conclusion

## Technologies Used
- numpy			: 1.26.4
- pandas		: 2.2.2
- seaborn		: 0.13.2
- matplotlib		: 3.9.0
- statsmodels		: 0.14.0
- sklearn		: 1.3.0
- scipy			: 1.11.1
- IPython		: 8.15.0
- ipykernel		: 6.25.0
- ipywidgets		: 8.0.4
- jupyter_client	: 7.4.9
- jupyter_core		: 5.3.0
- jupyter_server	: 1.23.4
- jupyterlab		: 3.6.3
- nbclient		: 0.5.13
- nbconvert		: 6.5.4
- nbformat		: 5.9.2
- notebook		: 6.5.4
- qtconsole		: 5.4.2
- traitlets		: 5.7.1
- conda			: 23.7.4

## Conclusions
**From the Exploratory Data Analysis , we can conclude the following -**
- Bike rental counts are lowest in spring and highest in fall, with summer showing significantly peak rentals.
- There was an increase in bike rentals in 2019 compared to 2018.
- Data for heavy_snow_rain weather situations is missing, potentially affecting analysis of extreme weather impacts.
- Bike rentals peak in June, July, and September, with lower counts in January.
- More bike rentals occur on working days compared to non-working days.
- Rental counts are higher on non-holidays compared to holidays.
- Rental demand remains consistent across all weekdays.
- Favorable weather "Clear Sky" correlates with higher rental counts, while poor weather "Light snowy rain" correlates with lower counts. There is no occurance for "Heavy snowy rain".
- Strong positive correlations exist between temperature (temp/atemp) and rental counts.
- Registered users show a strong positive correlation with rental counts.
- Casual users also positively correlate with rental counts, though less strongly than registered users.
- Humidity and windspeeds show weak correlations with rental counts and other variables.
- Humidity and windspeeds show weak correlations with rental counts and other variables.
- Bike rentals increase from March to June and decrease towards the end of the year.
- Higher temperatures (temp/atemp) positively influence rental counts.

**Q : Which variables are significant in predicting the demand for shared bikes? How Well the Significant Variables Describe Bike Demand ?**
- High R-squared: The model explains 84.29% of the variance in bike demand for the training set and 80.51% for the test set, indicating a strong fit.
- Temperature: There is a strong positive relationship, with higher temperatures significantly increasing bike demand.
- Year (2019): Shows a substantial increase in bike demand in 2019 compared to 2018, indicating a growing trend.
- Weather Conditions: Adverse weather reduces demand, especially during light snow/rain and misty conditions.
- Windspeed and Humidity: Both negatively impact demand, with higher windspeed and humidity levels leading to decreased bike usage.
- Seasonal Effects: Higher demand is observed in Fall , Summer and Winter.
- Monthly Effects: Lower demand in January and July, higher demand in September.
- Weekday Monday: Positive effect on bike demand.
- Working Day: Increases bike demand.

## Acknowledgements

- The project reference course materieals from upGrads curriculm .
- The project references from presentation in upgrad live class given by [Shivam Garg]

## Glossary

- Data Visualization
- EDA (Exploratory Data Analysis)
- Feature Scaling (Normalization)
- Dummy Variable (One Hot Encoding)
- Linear Regression
- p-value and Confidence Interval
- Coefficient of Determination (R²) and Adjusted R²
- Mean Squared Error (MSE) and Root Mean Squared Error (RMSE)
- Cross-Validation
- Multicollinearity
- Residuals Analysis

## Author
* [Avinash Vishwakarma]
