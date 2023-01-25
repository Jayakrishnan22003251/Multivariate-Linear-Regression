# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd

### Step2
Read the CSV file

### Step3
Get the values of X and Y variables

### Step4
create the linear regression model and fit

### Step5
predict the co2 emission of a car where the weight is 2300kg,and the volume is 1300cm cube

## Program:
```
Developed by:JAYAKRISHNAN L B L
Reg.No: 22003251
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
## Output:

![image](https://user-images.githubusercontent.com/120232371/214654728-c47a7d24-f6ad-4182-8e93-613456595a4a.png)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
