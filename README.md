# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import the required libraries pandas and LinearRegression from sklearn.
Read the dataset file "car (1).csv" using pd.read_csv() and store it in a dataframe.
### Step2
Select the independent variables Volume and Weight as input data x.
Select the dependent variable CO2 as output data y.
### Step3
Create a linear regression model using LinearRegression()..Train the model using fit(x, y).
### Step4
Display the regression coefficients using coef_.
Display the intercept value using intercept_.
### Step5
Predict the CO2 emission for the values Volume = 3300 and Weight = 1300 using predict().
Display the predicted result.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))
```
## Output:
<img width="843" height="375" alt="image" src="https://github.com/user-attachments/assets/3df221d5-e11c-4410-8684-37a424d919d6" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
