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

<img width="616" height="471" alt="598156981-74cca7b1-28ea-4e85-8221-8943a2a2648a" src="https://github.com/user-attachments/assets/cedc3820-e5dd-4313-aeac-1ed8ec04ef56" />


## Program:
```
import numpy as np
from sklearn.linear_model import LinearRegression

X = np.array([[1, 1], [1, 2], [2, 2], [2, 3]])
y = np.dot(X, np.array([1, 2])) + 3

reg = LinearRegression().fit(X, y)

reg.score(X, y)

print('Coefficients: ', reg.coef_)
print('Intercept: ', reg.intercept_)

print('Prediction: ', reg.predict(np.array([[3, 5]])))







```
## Output:
<img width="616" height="471" alt="598156981-74cca7b1-28ea-4e85-8221-8943a2a2648a" src="https://github.com/user-attachments/assets/4cc705d1-ab83-4f1e-b97d-96c0486e4d4c" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
