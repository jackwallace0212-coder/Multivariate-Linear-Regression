# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import the required libraries numpy and LinearRegression.
### Step2
Create the input data X and output data y using NumPy arrays.

### Step3
Create the Linear Regression model and train it using the fit() method.

### Step4
Display the coefficient and intercept values of the trained model.

### Step5
Predict the output for the new input [[3,5]] using the predict() method and display the result.



## Program:
```
Developed by: SARANYA R
Register Number: 212225040384

import pandas as pd
from sklearn import linear_model

df = pd.read_csv("car.csv")

X = df[['Weight', 'Volume']]
y = df['CO2']

regr = linear_model.LinearRegression()
regr.fit(X, y)

print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)

predictedCO2 = regr.predict(pd.DataFrame([[3300, 1300]], columns=['Weight', 'Volume']))
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)

```
## Output:

<img width="693" height="64" alt="image" src="https://github.com/user-attachments/assets/ce528863-c8df-4294-8b97-1a1a00aeafa5" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
