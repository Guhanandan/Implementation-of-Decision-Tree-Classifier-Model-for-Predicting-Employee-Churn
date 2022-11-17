# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:

To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:

Hardware – PCs
Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm:

1.Import the standard libraries.

2.Upload the dataset and check for any null values using .isnull() function.

3.Import LabelEncoder and encode the dataset.

4.Import DecisionTreeClassifier from sklearn and apply the model on the dataset.

5.Predict the values of array. 

6.Import metrics from sklearn and calculate the accuracy of the model on the dataset. 

7.Predict the values of array. 8.Apply to new unknown values.

## Program:
~~~
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Guhanandan V
RegisterNumber: 212221220014

import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
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

~~~

## Output:

### DATA HEAD
![61](https://user-images.githubusercontent.com/100425381/202353839-3a5a2129-fcbd-4838-a16c-c32778fcf93c.png)


### DATA INFO
![62](https://user-images.githubusercontent.com/100425381/202353858-176b332e-00d7-431b-868b-41ded293b1a1.png)


### DATA ISNULL
![63](https://user-images.githubusercontent.com/100425381/202353964-13dca543-73c5-4821-9363-21de15df21ee.png)


### DATA LEFT

![64](https://user-images.githubusercontent.com/100425381/202354011-e83f2cb6-a07d-42fc-b32e-03002158fb59.png)

### X HEAD

![65](https://user-images.githubusercontent.com/100425381/202354014-a7ad5b6f-7c04-47f0-a819-55ebc47bfee6.png)

### DATA FIT

![66](https://user-images.githubusercontent.com/100425381/202354019-81758af6-edbb-4823-bb9a-efeb26e25302.png)

### ACCURACY

![67](https://user-images.githubusercontent.com/100425381/202354024-50fc2678-4a15-4b0c-aafb-afe401cc4c61.png)

### PREDICTED VALUES

![68](https://user-images.githubusercontent.com/100425381/202354210-4d588a5b-d8da-4793-b44b-a84aed31d932.png)


##Result:
Thus the program to implement the Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
