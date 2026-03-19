# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: R.Divyadharshini
RegisterNumber:  212225230062
import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
y=data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:
<img width="1002" height="317" alt="Screenshot 2026-03-19 114832" src="https://github.com/user-attachments/assets/e07e6327-b690-420d-b910-82e0041b219f" />
<img width="1064" height="274" alt="Screenshot 2026-03-19 114843" src="https://github.com/user-attachments/assets/df1737ef-c24d-497e-bc73-d9d6e0afe2be" />
<img width="637" height="285" alt="Screenshot 2026-03-19 114856" src="https://github.com/user-attachments/assets/75ef6ed5-82ea-4af5-8e53-6d27ea19bae5" />
<img width="630" height="41" alt="Screenshot 2026-03-19 114907" src="https://github.com/user-attachments/assets/fa3a1504-c2c9-46e4-aab8-1b84d54c36e9" />
<img width="1077" height="464" alt="Screenshot 2026-03-19 114920" src="https://github.com/user-attachments/assets/9214e992-be25-490b-bb6d-78915f3fafbd" />







## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
