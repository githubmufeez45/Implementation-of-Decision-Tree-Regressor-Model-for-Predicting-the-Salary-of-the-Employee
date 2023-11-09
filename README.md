# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the libraries and read the data frame using pandas.
2.Calculate the null values present in the dataset and apply label encoder.
3.Determine test and training data set and apply decison tree regression in dataset.
4.Calculate Mean square error,data prediction and r2.

## Program:
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: SHAIK MUFEEZUR RAHAMAN
RegisterNumber:  212221043007

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

## Output:
data.head():
![280364096-bf268109-2c11-4344-bd04-34dbc04ae63a](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134826568/4da9edd4-5eaf-4e7c-a928-006c6ed140f6)

data.info():
![280364233-aec7ab1b-a460-48d0-817d-79b8aecaf5f2](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134826568/0d80b166-7017-46a4-a88b-b2681a30b399)

isnull() and sum():
![280364387-98a398f7-16c5-44de-bd7a-a3c1589bb00d](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134826568/62adc884-449b-4bad-b8da-c96a6d189417)

data.head() for salary:
![280364476-fd74a5ce-5d26-4d67-8a09-5ddac083b3b9](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134826568/98477e6f-5477-4ab3-845a-63c78e5468ee)

MSE value:
![280364558-237f43c9-1073-4355-b7ba-0b0db25966fc](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134826568/d93bba2a-0034-4015-b19a-2984ea99ed4a)

r2 value:
![280364623-cc4a09c5-2f73-45c4-b237-7935dddb6409](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134826568/0b398b28-97c5-4336-96ce-a7835b574ed0)

data prediction:
![280364681-d3612ae9-97a2-4ba9-9708-97aa30ce02c4](https://github.com/githubmufeez45/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/134826568/1a6de12d-cfef-48c4-a279-abe580e324ba)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
