# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
 Import pandas module. Import linear_model from sklearn

### Step2
Read the csv file (saved in the same directory) using pd.read_csv

### Step3
Prepare regression using linear_model.LinearRegression() and assign it to identifier
 "regr"

### Step4
The coefficients can be obtained by regr.coef_ and the intercept can be obtained by
 regr.intercept_. The predicted result can be obtained by regr.predict()

### Step5
Print the output and end the program

## Program:
```
 import pandas as pd
 from sklearn import linear_model
 df = pd.read_csv("carsemission.csv")
 X = df[['Weight', 'Volume']]
 y = df['CO2']
 regr = linear_model.LinearRegression()
 regr.fit(X, y)
 print('Coefficients:', regr.coef_)
 print('Intercept:',regr.intercept_)
 predictedCO2 = regr.predict([[3300, 1300]])
 print('Predicted CO2 for the corresponding weight and volume',predictedCO2)

```
### Output:
![Screenshot 2024-12-14 101728](https://github.com/user-attachments/assets/f83666e5-300e-4a69-89d2-6de1f6546751)

### Insert your output:

![Screenshot 2024-12-14 101739](https://github.com/user-attachments/assets/a762e774-5fc7-4d66-9cde-6bc3bc9fd585)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
