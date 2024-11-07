# DATE:
# EXP.NO.10 Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd

### Step2
Read the csv file

### Step3
Get the value of x and y variables

### Step4
Create the linear regression model and fit

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

## Program:
```
Developed by:MOHAN S 
Register number: 212223240094

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO@ for the corresponding weight and volume",predictedCO2)


```
## Output:
### Insert your output
![Screenshot 2024-11-07 213903](https://github.com/user-attachments/assets/4f43ab83-e6d7-4294-8705-f97ddd8c905a)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
