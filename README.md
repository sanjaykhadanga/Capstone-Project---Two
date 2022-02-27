# Bike Sharing Demand Prediction
Capstone-Project---Two

Currently rental bikes are introduced in many urban cities for the enhancement of mobility comfort. The purpose of this movement is to modernize cities and encourage people to head to a green world. Let's take the examples of Paris in 2007, where "velibs" were introduced and Amsterdam, where there are more bikes than cars. The goal is to facilitate the commute in the Seoul and reduce the amount of cars and the pollution. Indeed, the development of the way to commute reduced the use of cars to go to work and visit the city.

It is important to make the rental bike available and accessible to the public, as it provides many alternatives to commuters in metropolises. There are a lot of advantages to bike rents, it is convenient because it permits people not to keep the bike all day long, whether it is at work or at school. Furthermore it is the healthiest way to travel and it has many environmental benefits.

The studied dataset contains weather information which are the features (Temperature, Humidity, Wind speed, Visibility, Dew point, Solar radiation, Snowfall, Rainfall), the target is the number of bikes rented per hour and date information. The dataset presents the company's data between December the 1st of 2017 and finishes one year later.

**How many bikes are rented per hour in function of weather conditions ?**

The goal of the company Seoul Bike is providing the city with a stable supply of rental bikes. It becomes a major concern to keep user satisfied. The crucial part is the prediction of bike count rents at each hour for a stable supply of rental bikes. We can suppose that this study could be reported to the company 'Seoul Bikes'. We think it could help them knowing if yes or not they have to supply bikes stations in the city, in order to keep a good satisfaction of the customers.

You can find the dataset necessary for the analysis on following link : https://archive.ics.uci.edu/ml/datasets/Seoul+Bike+Sharing+Demand#

**Data Description**

The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour, and date information.

Attribute Information:
Date : year-month-day
Rented Bike count - Count of bikes rented at each hour
Hour - Hour of he day
Temperature-Temperature in Celsius
Humidity - %
Windspeed - m/s
Visibility - 10m
Dew point temperature - Celsius
Solar radiation - MJ/m2
Rainfall - mm
Snowfall - cm
Seasons - Winter, Spring, Summer, Autumn
Holiday - Holiday/No holiday
Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)

**Steps involved:**

The following steps are involved in the 
project

**1. EXPLORATORY DATA ANALYSIS :** 

After loading and reading the dataset in the notebook, we performed EDA. Comparing target variable which is bike rentals counts with other independent variables. This process helped us figure out various aspects and relationships among the target and the independent variables and also we observed the distribution of variables. It gave us a better idea that how the feature behaves with the target variable.

**2. NULL VALUES TREATMENT AND OUTLIERS :**

The dataset contains no null values to disturb the accuracy but outliers are present which can disturb the accuracy. So Again, we use a zscore to remove outliers.

**3. NUMERICAL AND CATEGORICAL FEATURES:**

With the help of exploratory data analysis we analyzed the categorical as well as numerical features in the dataset.

**4. ONE HOT ENCODING :**

In this dataset some categorical variables like seasons, holidays,and function days, we change with a numerical database.

**5. CORRELATION ANALYSIS :**

We plot the heat map to find the correlation between both the dependent variable and independent variables.

**6. TRAIN TEST SPLIT :**

In the train test split, we take x as dependent variables and y take as an independent variable then train the model.

**7. MODELS :**

We use 4 models to train the data 
and for predicting the accuracy, 
RMS and R2. 

1. Linear regression
2. Lasso regression
3. Ridge regression
4. Elastic net
5. Decision tree
6. Random forest
7. Gradient boostin
8. 
**HYPERPARAMETER TUNING:**

Before proceeding to try the next models, let us try to tune some hyperparameters and see if the performance of our model improves.

**USING GridSearchCV:**

GridSearchCV helps to loop through predefined hyperparameters and fit the model on the training set. So, in the end,we can select the best parameters from the listed hyperparameters

**Conclusion**


• The Rented Bike Count has been increased from 2017 to 2018.

• No overfitting is seen.

• XGBoost Regressor gives the highest R2 score of 96.6% for Train Set and 89.4% for Test set.

• Feature Importance value for Random Forest, Gradient Boost, and XGBoost are different.

• We can deploy this model.
