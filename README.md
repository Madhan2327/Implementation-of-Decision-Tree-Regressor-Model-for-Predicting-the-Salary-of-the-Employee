# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas
2. Import Decision tree classifier
3. Fit the data in the model
4. Find the accuracy score
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by:MADHAN C
RegisterNumber:24004329
import pandas as pd
from sklearn.tree import DecisionTreeClassifier,plot_tree
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
y=data["left"]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
plt.figure(figsize=(8,6))
plot_tree(dt,feature_names=x.columns,class_names=['salary','left'],filled=True)
plt.show()
*/
```

## Output:
![Decision Tree Regressor Model for Predicting the Salary of the Employee](sam.png)
![Screenshot 2024-11-28 212746](https://github.com/user-attachments/assets/eeb1eeea-3a35-41b3-be3e-630440b27ab5)
![Screenshot 2024-11-28 213038](https://github.com/user-attachments/assets/8523b503-398e-4a52-a64b-510040575d25)
![Screenshot 2024-11-28 213046](https://github.com/user-attachments/assets/4fd5df12-760d-4f48-87af-8993339b4f12)
![Screenshot 2024-11-28 213050](https://github.com/user-attachments/assets/16ba9c0c-11b1-48b8-9c69-a87f756f752b)
![Screenshot 2024-11-28 213412](https://github.com/user-attachments/assets/6f865675-8ca7-457d-a3f4-9098ac397fdc)
![Screenshot 2024-11-28 213447](https://github.com/user-attachments/assets/352647b4-e64e-4915-9e84-700f9b0c9291)
![Screenshot 2024-11-28 213536](https://github.com/user-attachments/assets/6b16d08a-388f-46d5-b5ee-cf86df0f5504)
![Screenshot 2024-11-28 213652](https://github.com/user-attachments/assets/27ae2a3b-a688-4165-a2c8-256f1fa68631)
## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
