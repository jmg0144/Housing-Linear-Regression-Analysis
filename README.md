# Home Sales Analysis Project
Author: Justin Giovatto
## Overview
This project analyzes data from a King County house sales dataset. The data will be used to create a linear model that will be used to predict home prices as accurately as possible.  
## Business Problem
Hypothetical Situation: A King County real estate agency is looking to help potential clients determine the true value of their home through the use of a linear model. 

## Data
I will analyze data from the King County house sales dataset below 

kc_house_data.csv

Contains data on King County homes including:

* id - unique identified for a house

* dateDate - house was sold

* pricePrice - is prediction target

* bedroomsNumber - of Bedrooms/House

* bathroomsNumber - of bathrooms/bedrooms

* sqft_livingsquare - footage of the home

* sqft_lotsquare - footage of the lot

* floorsTotal - floors (levels) in house

* waterfront - House which has a view to a waterfront

* view - Has been viewed

* condition - How good the condition is ( Overall )

* grade - overall grade given to the housing unit, based on King County grading system

* sqft_above - square footage of house apart from basement

* sqft_basement - square footage of the basement

* yr_built - Built Year

* yr_renovated - Year when house was renovated

* zipcode - zip

* lat - Latitude coordinate

* long - Longitude coordinate

* sqft_living15 - The square footage of interior housing living space for the nearest 15 neighbors

* sqft_lot15 - The square footage of the land lots of the nearest 15 neighbors

![Screen Shot 2021-09-14 at 8 48 15 AM](https://user-images.githubusercontent.com/66973223/133267229-bb7ed2f6-2e06-45ed-b9a6-0e4ef2ca689e.png)

![Screen Shot 2021-09-14 at 8 48 37 AM](https://user-images.githubusercontent.com/66973223/133267918-8bab9ed5-b691-4988-b5bb-e959037658c6.png)

## Methods
Using specific columns from the data provided I will build four unique linear models using different features from the data provided. I will then split the data into training and testing data. The models will be trained using the training data and then evaluated on the testing data to determine their accuracy. The accuracy of these models will be determined mainly by r-squared, mean absoluate error, mean squared error, and root mean squared error. After determining the accuracy of these model I will then evaluate the coefficients in order to determine which features are most important in determining true home value.   

## Results & Conclusions  

The final model on average was able to predict home prices within $77,528 of the true home price. The R-squared for the final model was .801, with a Skew of 1.324, and Kurtosis of 9.326. The model also produced a Mean Squared Error of 12,404,565,078 as well as a Root Mean Squared Error of 111,375.

![Screen Shot 2021-09-14 at 8 50 44 AM](https://user-images.githubusercontent.com/66973223/133268182-e22ce18b-e34a-4fbe-9efc-196dc63bddcd.png)

Based on the analysis, my main business recommendations are as follows:

1. Zip Codes appear to be the most important feature in determining true home value according to the models.
2. Square foot living/square foot above/sum square foot living tend to be the second most important feature.
3. Bathrooms and Home Grade also appear to be fairly significant features in determining home price.

![Screen Shot 2021-09-14 at 9 41 39 AM](https://user-images.githubusercontent.com/66973223/133268501-d0455151-0920-4316-a5a6-479269acc4c1.png)

![Screen Shot 2021-09-14 at 8 51 35 AM](https://user-images.githubusercontent.com/66973223/133268263-23ca16c3-05d3-4e6a-b423-ea6e6da2adc5.png)

![Screen Shot 2021-09-14 at 8 51 48 AM](https://user-images.githubusercontent.com/66973223/133268314-f2834f39-0711-4f43-ac75-b6d25b9ffeac.png)

## For More Information
See the full analysis in the [Jupyter Notebook](https://github.com/jmg0144/home-sales-analysis/blob/main/home-sales-analysis.ipynb) 

For additional information contact Justin Giovatto at justin.giovatto@gmail.com

## Repository Structure
├── data

├── README.md

├── Home_Sales_Analysis_Presentation.pdf

└── home-sales-analysis.ipynb
