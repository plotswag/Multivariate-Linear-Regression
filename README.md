# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import panda
### Step2
Import linear model from sklearn
### Step3
Read the file cars.csv
### Step4
Assign the values for x and y as required
### Step5
Create the linearRegression model and predict the output
## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:", regr.coef_)
print("Intercept:", regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predictedd co2 for the corresponding weight and volume", predictedCO2)
```
## Output:
![image](https://github.com/plotswag/Multivariate-Linear-Regression/assets/145822344/7ce8bb19-468d-4c6c-a670-f52f17915486)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
