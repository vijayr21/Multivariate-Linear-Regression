# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import panda

### Step2
import linear mode; from sklearn

### Step3
Read the file cars.csv

### Step4
Assign the values for x and y as required

### Step5
Create the linearRegression model and predict the output

## Program:
```
#Developed by :VIJAY R
#Register number:- 23013759
import pandas as pd
from sklearn import linear_model

df = pd.read_csv('cars.csv')
X = df[['Weight','Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X,y)
print("Cofficients: ",regr.coef_)
print("Intercept: ",regr.intercept_)
predictedCO2 = regr.predict([[3300,1300]])
print('Predicted co2 for the corresponding weight and volume',predictedCO2)

```
## Output:

### Insert your output
![maths 10](https://github.com/vijayr21/Multivariate-Linear-Regression/assets/149347607/1882354a-d443-440f-9b89-0c5de2b3dec7)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
