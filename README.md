# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

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
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: YUVARAJ B
RegisterNumber:  212222040186

import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()    #no departments and no left
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
*/
```

## Output:
#### data.head()
![Screenshot 2024-04-06 202922](https://github.com/rohithprem18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/146315115/3b6d1584-564f-4ff4-92e1-9e72a4bfd271)

#### data.info()
![Screenshot 2024-04-06 202927](https://github.com/rohithprem18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/146315115/6fd24494-3daa-4454-b74d-4705f541bc06)

#### isnull() and sum()
![Screenshot 2024-04-06 202931](https://github.com/rohithprem18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/146315115/0bbc04b9-2b96-477b-bad1-d910d204480e)

#### data value counts()
![Screenshot 2024-04-06 202936](https://github.com/rohithprem18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/146315115/07ba789e-e175-4018-bfd2-548037bbb6ba)

#### data.head() for salary
![Screenshot 2024-04-06 202941](https://github.com/rohithprem18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/146315115/fbd2b025-c2e6-42fa-9cfa-a62d95e04829)

#### x.head()
![Screenshot 2024-04-06 202946](https://github.com/rohithprem18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/146315115/e6eebae1-b13f-4a4d-8552-2af070534275)

#### accuracy value
![Screenshot 2024-04-06 202950](https://github.com/rohithprem18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/146315115/36a73dd2-3b0e-4111-9cca-a92defe90f1d)

#### data prediction
![Screenshot 2024-04-06 202956](https://github.com/rohithprem18/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/146315115/5226bebe-5fc8-462c-b235-aafed67fc98f)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
