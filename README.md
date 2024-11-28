# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import pandas
2.Import Decision tree classifier
3.Fit the data in the model
4.Find the accuracy score
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by:MADHAN C 
RegisterNumber:24004329
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
x.head()
y=data["Salary"]
y.head()
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
y_pred
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])  
*/
```

## Output:
![Decision Tree Regressor Model for Predicting the Salary of the Employee](sam.png)
![Screenshot 2024-11-28 215827](https://github.com/user-attachments/assets/9079a949-e108-4b40-ad0a-735c03b70501)
![Screenshot 2024-11-28 215851](https://github.com/user-attachments/assets/4519eee5-c937-45a1-8c97-ddc6e58dbb0e)
![Screenshot 2024-11-28 215918](https://github.com/user-attachments/assets/8510d971-1a9f-4891-bcba-769c1c1bc9b5)
![Screenshot 2024-11-28 215958](https://github.com/user-attachments/assets/43c81b51-0939-455c-8419-075bbd23b40b)
![Screenshot 2024-11-28 220102](https://github.com/user-attachments/assets/93fbd0c8-2a70-4c02-bdab-8fe198f61459)
![Screenshot 2024-11-28 220134](https://github.com/user-attachments/assets/2fc23862-f3f7-41db-9d11-bccdfe87718c)
![Screenshot 2024-11-28 220233](https://github.com/user-attachments/assets/161ed3b4-c984-410d-9b72-76d3999d0263)
![Screenshot 2024-11-28 220405](https://github.com/user-attachments/assets/05d8cd3d-6d21-45be-89d3-fbf856a5e324)
![Screenshot 2024-11-28 220353](https://github.com/user-attachments/assets/37eab133-7aaa-4808-bd3a-95362f3e0a23)
## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
