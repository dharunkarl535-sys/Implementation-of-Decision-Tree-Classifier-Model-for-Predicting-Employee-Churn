# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

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
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: 
RegisterNumber:
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
import pandas as pd
data=pd.read_csv("Employee.csv")
print("data.head():")
data.head()
print("data.info():")
data.info()
print("isnull() and sum():")
data.isnull().sum()
print("data value counts():")
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
print("data.head() for Salary:")
data["salary"]=le.fit_transform(data["salary"])
data.head()
print("x.head():")
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
print("Accuracy value:")
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
print("Data Prediction:")
dt.predict([[0.5,0.8,9,260,6,0,1,2]])
from sklearn.tree import plot_tree
import matplotlib.pyplot as plt

plt.figure(figsize=(8,6))
plot_tree(dt, feature_names=x.columns, class_names=['salary', 'left'], filled=True)
plt.show()
Developed by:Girishva.K 
RegisterNumber:25009292 
*/
*/
```

## Output:
![decision tree classifier model](sam.png)
<img width="1232" height="228" alt="530316845-3f440b47-b31b-4ad2-b4b4-72bac9138d8d" src="https://github.com/user-attachments/assets/748af1df-1cd4-4541-a7d7-c5f991575b59" />
<img width="980" height="366" alt="530316907-f72bbff5-ed4e-43ec-949e-5d6233ce20d3" src="https://github.com/user-attachments/assets/df5674d3-5c42-44e2-ab50-0bdbf342e944" />
<img width="843" height="257" alt="530316960-349f9ec0-8b7f-45fe-bf15-a78106aad599" src="https://github.com/user-attachments/assets/9eba0c5f-d4ce-4d68-a584-7430ce15b5f5" />
<img width="501" height="120" alt="530316984-ff9661d9-6fe9-4686-b20b-19569732e3db" src="https://github.com/user-attachments/assets/d64968c0-5270-4265-8c0f-e32e56bf6572" />
<img width="1247" height="223" alt="530317012-76601ef8-e31d-4c0d-9696-7b42e510e3f8" src="https://github.com/user-attachments/assets/cac4c13d-32aa-49b5-b698-dcc2e31d9914" />
<img width="1226" height="222" alt="530317054-86d764d4-de4a-499d-87e4-9e8417de7b02" src="https://github.com/user-attachments/assets/d37fab6c-7c9e-4117-b347-342f56350540" />
<img width="1226" height="222" alt="530317054-86d764d4-de4a-499d-87e4-9e8417de7b02" src="https://github.com/user-attachments/assets/ca3fae26-2406-4091-a3d4-5a692e9a8241" />
<img width="452" height="65" alt="530317166-0da5fc56-e4f1-46fa-a724-e38b5fb4a9f6" src="https://github.com/user-attachments/assets/e4d81f7f-3b77-4ed2-8942-6fe816ae59dd" />
<img width="1247" height="133" alt="530317209-6adfd144-bdd3-4cd6-892e-41cd0b32f033" src="https://github.com/user-attachments/assets/4acf1086-10e6-4fbd-b193-ec7afa6ec3a7" />
![Uploading 530317248-74440b99-f3e9-434d-b976-5f7e10010478.png…]()


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
