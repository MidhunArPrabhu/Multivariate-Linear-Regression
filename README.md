# EXPERIMENT-10
# IMPLEMENTATION OF MULTIVARIATE LINEAR REGRESSION 

## AIM :

To write a python program to implement multivariate linear regression and predict the output.

## EQUIPMENYS REQUIRED :

-	Hardware – PCs
-	Anaconda – Python 3.7 Installation / Moodle-Code Runner

## ALGORITHIM :

### STEP 1 :

import pandas as pd.

### STEP 2 :

Read the csv file.

### STEP 3 :

Get the value of X and y variables.

### STEP 4 : 

Create the linear regression model and fit.

### STEP 5 :

Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

### STEP 6 :

Print the predicted output.

## Program:
```python
# Developed by : MIDHUN AZHAHU RAJA P
# Register No : 22008311

import pandas as pd
from sklearn import linear_model
data= pd.read_csv("cars.csv")

X=data[['Weight','Volume']]
Y=data['CO2']

regr=linear_model.LinearRegression()
regr.fit(X,Y)

print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)

predictCO2=regr.predict([[3300,1300]])
print("prediction CO2 for the corresponding weight and volume",predictCO2)



```
## OUTPUT :
![loop](https://user-images.githubusercontent.com/118054670/214789949-ed930578-45fd-485e-bb3f-6a9658434c7e.png)


## RESULT :

Thus the multivariate linear regression is implemented and predicted the output using python program.
