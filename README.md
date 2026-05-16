# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd.

### Step2
Read the csv file.

### Step3
Get the value of X and y variables

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

## Program:
```
Developed by : Girishva.k
Reg No : 212225040094
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

### Insert your output

<img width="912" height="93" alt="592917146-37722f12-4f10-45a0-8c2e-37718523f328" src="https://github.com/user-attachments/assets/041fe811-f840-43e0-9431-d58df9137449" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
