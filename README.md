# King County Home Value Analysis
Author: Justin Giovatto
## Overview
This notebook will analyze data from the King County House Sales dataset. This dataset contains various information on homes in King County, Washington. I will use this data in order to create linear regression models with the purpose of determining which features are most relevant in predicting home values. I will then examine the models' output and compare and contrast to determine which model performs best according to the R-Squared and Mean Absolute Error metrics. 
## Business Problem
Hypothetical Situation: A King County real estate agency is looking to provide advice to home owners on what factors are most important in determining the value of their home. Using several multiple linear regression models I will examine which independant variables are most useful at predicting the dependant variable of home price. The regression models will help in providing home owners with relevant information regarding the price of their home should they be interested in listing their home with the real estate agency.  

## Data
Data from the King County house sales dataset contains the following information regarding homes in King County: 

* id - unique identifier for a home

* dateDate - date home was sold

* pricePrice - home sale price

* bedroomsNumber - number of bedrooms

* bathroomsNumber - number of bathrooms

* sqft_livingsquare - footage of the home

* sqft_lotsquare - footage of the lot

* floorsTotal - total number of levels in home

* waterfront - home which has a view to a waterfront

* view - has been viewed by potential buyers

* condition - overall condition of the home

* grade - overall grade given to the housing unit, based on King County grading system

* sqft_above - square footage of house apart from basement

* sqft_basement - square footage of the basement

* yr_built - year home was built

* yr_renovated - year home was renovated

* zipcode - zip

* lat - Latitude coordinate

* long - Longitude coordinate

* sqft_living15 - square footage of interior housing living space for the nearest 15 neighbors

* sqft_lot15 - square footage of the land lots of the nearest 15 neighbors

![Screen Shot 2021-11-11 at 10 00 12 AM](https://user-images.githubusercontent.com/66973223/141325768-e5559cdd-e573-4381-9f1c-5f25c6dbbe8d.png)

![Screen Shot 2021-11-11 at 10 18 28 AM](https://user-images.githubusercontent.com/66973223/141325822-7a2c8567-eeda-457c-84be-194286ede13e.png)

![Screen Shot 2021-11-11 at 10 00 24 AM](https://user-images.githubusercontent.com/66973223/141325861-50c19aca-5e95-4270-ae8d-46d6cae85c00.png)


## Methods
Using columns from the data provided I will build four unique linear models. I will then split the data into training and testing data. The models will be trained using the training data and then evaluated on the testing data to determine their accuracy. The accuracy of these models will be determined mainly by r-squared, mean absoluate error, mean squared error, and root mean squared error. After determining the accuracy of these model I will then evaluate the coefficients in order to determine which features are most important in determining true home value.

![Screen Shot 2021-11-11 at 10 00 47 AM](https://user-images.githubusercontent.com/66973223/141325939-00d9b756-20df-4752-9ed7-c95a400aa9a7.png)

![Screen Shot 2021-11-11 at 10 39 56 AM](https://user-images.githubusercontent.com/66973223/141326061-a6f9691f-7c9d-4e3a-b747-117bf2e3ae35.png)

![Screen Shot 2021-11-11 at 10 01 21 AM](https://user-images.githubusercontent.com/66973223/141326213-e22d39fb-d38a-4ec7-9973-c7f83b3090e7.png)

![Screen Shot 2021-11-11 at 10 41 41 AM](https://user-images.githubusercontent.com/66973223/141326319-a8bbb5dd-fb0a-4d7a-b57c-ab02a8cacd71.png)

![Screen Shot 2021-11-11 at 10 43 01 AM](https://user-images.githubusercontent.com/66973223/141326600-1d716403-525c-43fa-805f-e1264a59f118.png)

![Screen Shot 2021-11-11 at 10 43 14 AM](https://user-images.githubusercontent.com/66973223/141326646-e41f727f-ae2a-4343-abe5-1937d7d32420.png)

![Screen Shot 2021-11-11 at 10 43 27 AM](https://user-images.githubusercontent.com/66973223/141326678-ca05176d-db42-468d-8a13-a8de352a0cc5.png)

![Screen Shot 2021-11-11 at 10 43 37 AM](https://user-images.githubusercontent.com/66973223/141326707-ff29c570-0257-4c06-ab7e-20135fcd604d.png)

## Results & Conclusions  

The most reliable model was Model D which was able to predict home prices within $106,695 of the true home price. The R-squared for Model D was .655, with a Skew of 1.181, and Kurtosis of 6.691. Model D also produced a Mean Squared Error of 21,624,092,902 as well as a Root Mean Squared Error of 147,051.

While Models B and C produce the highest R-Squared metric, they also have a high skew and kurtosis likely due to the presence of outliers as well as the uneven distribution of homes within the zip code categorial columns. Once the outliers and zip code columns were removed for Model D, both the skew and kurtosis significantly decreased making for a more reliable model.

Aside from zip codes; Square Foot Living, Grade, and Year Built all appear in the top three features for multiple models making these features the most important in predicting home price according to the models. Also once zip codes were replaced with the new 'Distance from Seattle' feature in Model D, we can see that this feature ranked second in terms of importance.

According to the models we can infer that home size, location, age, and 'grade' are the most important features in accurately predicting home value for King County.

![Screen Shot 2021-11-11 at 10 45 52 AM](https://user-images.githubusercontent.com/66973223/141327441-cbb71254-eefb-48dd-8f2d-6ce1535fe720.png)

![Screen Shot 2021-11-11 at 10 46 02 AM](https://user-images.githubusercontent.com/66973223/141327529-b6b306b2-4386-4739-91e1-6c355f036de5.png)

![Screen Shot 2021-11-11 at 10 46 18 AM](https://user-images.githubusercontent.com/66973223/141327580-5fa81ce5-793c-4c7c-bbb1-f8387b6f4125.png)

![Screen Shot 2021-11-11 at 10 46 28 AM](https://user-images.githubusercontent.com/66973223/141327610-685ba56f-fee2-4c7d-83db-02bc07e99197.png)

![Screen Shot 2021-11-11 at 10 46 37 AM](https://user-images.githubusercontent.com/66973223/141327649-cb01690e-1de0-4a11-a6bb-ba229cad8076.png)

![Screen Shot 2021-11-11 at 10 46 46 AM](https://user-images.githubusercontent.com/66973223/141327678-95a29b4a-59a4-4582-b271-9fa5ac64e70d.png)

## For More Information
See the full analysis in the [Jupyter Notebook](https://github.com/jmg0144/home-sales-analysis/blob/main/home-sales-analysis.ipynb) 

For additional information contact Justin Giovatto at justin.giovatto@gmail.com

## Repository Structure
├── data

├── README.md

├── Home_Sales_Analysis_Presentation.pdf

└── home-sales-analysis.ipynb
