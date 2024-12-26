# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
```
Step1:
Import pandas
Step2:
Import linear model from sklearn
Step3:
Read the file cars.csv
Step4:
Assign the values for x and y as required
Step5:
Create the linearRegression model and predict the output
```

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("/content/drive/MyDrive/car (1).csv")
x=df[['Volume','Weight']]
y=df['CO2']
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))

```
## Output:
![alt text](image.png)

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.