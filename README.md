# Price-Prediction-of-pre-owned-cars

Case study: predicting the price of pre-owned cars. Unlike classification like classifying it under categories, here we are predicting the value. With the help of creating a model, we can predict the prices of the car.

Filename: cars_data.csv
Dataset size: 50,000 X 19  - 19 attributes among which one is the dependent variable.

Here the dependent variable is the price variable.

Things which we have to be done are,
		1. Identify if the data is clean.
		2. Check if the data is having any missing values.
		3. Then we look for variables variables influencing price and identify the relationship between the variables using correlation, scatter plot, etc.
		4. Identify outliers using central tendency measure, box plot, etc.
		5. Then look if categories with meagre frequencies can be combined so that we can combine it into a compact one.

Method Identification:
		1. Linear regression.
		2. Random Forest.
Inferences:
The metrics for model built from data where missing values were omitted:

R squared value for train data in Linear Regression : 0.780
R squared value for test data in Linear Regression  : 0.765
R squared value for train data in Random Forest : 0.92
R squared value for train data in Random Forest : 0.850
Base RMSE of model built from data where missing values where omitted : 1.127
RMSE value for test from Linear Regression: 0.5455
RMSE value for test from Random forest: 0.436


The metrics for model built from data where missing values were imputed:

R squared value for train data in Linear Regression : 0.707
R squared value for test data in Linear Regression  : 0.7023
R squared value for train data in Random Forest : 0.90
R squared value for test data in Random Forest :0.820
Base RMSE of model built from data where missing values where omitted : 1.188
RMSE value for test from Linear Regression: 0.648
RMSE value for test from Random forest: 0.494

From the inferences, we can come to a conclusion that random forest is far more effective than Linear Regression. Also, when computing by omitting the missing values, error rate is less than when computing by imputing the missing values. But if we notice, when omitting the missing values, we can see that nearly 10,000 records are getting omitted, so we shouldn't omit that large size because we may also get some information from those records.
