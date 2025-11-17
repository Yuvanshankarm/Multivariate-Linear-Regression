# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### Step1 : Import the Neccessary Libraries

### Step2 : Read car.csv into a DataFrame df.

### Step3 : Select inputs (features) and output (target)

### Step4 : Instantiate a linear regression model: regr = LinearRegression().

### Step5 : Print regr.coef_ and   Print regr.intercept_ 

### Step6 : Print the regr.predict([[3300, 1300]]) and the predicted CO₂ value.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
X = df[["Volume","Weight"]]
Y = df["CO2"]
regr = linear_model.LinearRegression()
regr.fit(X,Y)
print("Coefficient:",regr.coef_)
print("Intercept",regr.intercept_)
print("Predicting the CO2",regr.predict([[3300,1300]]))
```
## Output:


<img width="861" height="381" alt="image" src="https://github.com/user-attachments/assets/b5d3f9d9-4cba-4560-bab4-67ccc46bf7f1" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
