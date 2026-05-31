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
#Developed By:DEVENDRAN G
#Register Number:212225240030
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
<img width="1235" height="441" alt="Screenshot 2026-05-31 145451" src="https://github.com/user-attachments/assets/9e01494d-5d39-4fbc-ab06-58fa78b20907" />

### Insert your output

<br><img width="980" height="85" alt="image" src="https://github.com/user-attachments/assets/c528d324-e912-46f6-8d04-2b5c0e94d9f7" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
