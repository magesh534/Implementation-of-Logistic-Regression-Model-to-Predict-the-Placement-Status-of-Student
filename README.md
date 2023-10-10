# Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student

## AIM:
To write a program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

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
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.
Developed by: magesh v
RegisterNumber:  212222040092
import pandas as pd
data=pd.read_csv('/content/Placement_Data.csv')
data.head()

data1=data.copy()
data1=data1.drop(["sl_no","salary"],axis=1)#remove the specified row or column
data1.head()

data1.isnull().sum()

data1.duplicated().sum()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data1["gender"] = le.fit_transform(data1["gender"])
data1["ssc_b"] = le.fit_transform(data1["ssc_b"])
data1["hsc_b"] = le.fit_transform(data1["hsc_b"])
data1["hsc_s"] = le.fit_transform(data1["hsc_s"])
data1["degree_t"] = le.fit_transform(data1["degree_t"])
data1["workex"] = le.fit_transform(data1["workex"])
data1["specialisation"] = le.fit_transform(data1["specialisation"])
data1["status"] = le.fit_transform(data1["status"])
data1

x=data1.iloc[:,:-1]
x

y=data1["status"]
y

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state = 0)

from sklearn.linear_model import LogisticRegression
lr = LogisticRegression(solver="liblinear")
lr.fit(x_train,y_train)
y_pred = lr.predict(x_test)
y_pred

from sklearn.metrics import accuracy_score
accuracy = accuracy_score(y_test,y_pred)
accuracy

from sklearn.metrics import confusion_matrix
confusion = confusion_matrix(y_test,y_pred)
confusion

from sklearn.metrics import classification_report
classification_report = classification_report(y_test,y_pred)
print(classification_report)

lr.predict([[1,80,1,90,1,1,90,1,0,85,1,85]])

*/
```

## Output:
![271912178-db957f74-baeb-4d5b-af90-6fb6cffbcc2e](https://github.com/magesh534/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/135577936/c4603361-a589-4a4d-9454-adc780f5317a)

![271912273-d0e8e5ba-b389-4a6d-aca7-0d8921c68f0e](https://github.com/magesh534/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/135577936/6a05087a-896f-4dda-9183-117d0959c138)
![271912302-f9ee445f-723f-4bcb-af64-4c6650794984](https://github.com/magesh534/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/135577936/f15df1d5-ad1b-4207-9fb1-1ef4bec98351)

![271912327-87fac85d-e25d-4e1c-ae8b-decfc06152e1](https://github.com/magesh534/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/135577936/ec6f4dec-33eb-4213-9db7-826f3adc64c8)
![271912364-c222bd91-15f3-4c2f-808c-d0bf5c570b26](https://github.com/magesh534/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/135577936/85defd42-a247-4168-812c-e665dfd40f30)
![271912400-db107eaa-5c7d-4ad2-a482-810dbb3b8a51](https://github.com/magesh534/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/135577936/ce6b2dde-45b4-4095-9a07-e823550cb8df)
![271912424-6e23680a-570b-410b-b5bf-eb00cd489689](https://github.com/magesh534/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/135577936/f1eef88f-1fe9-4e55-92ba-d291dfe05bf4)
![271912456-f6d4f7b6-81a7-41d5-a1c9-4cbc08cb17fa](https://github.com/magesh534/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/135577936/4e9d873c-53db-4c48-aaf9-d17c864bcb46)
![271912474-b2748076-f9fa-4aa9-9d7b-b8d175cc3d10](https://github.com/magesh534/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/135577936/edc84ac3-fa66-4b6b-a67c-e71f61e8e456)
![271912498-4cfde0fa-6aae-4184-bb3f-d057535f10b2](https://github.com/magesh534/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/135577936/dd5ee355-0cde-41f6-a5c2-3d5e3a9b867e)
![271912524-34c167a6-c0e3-4ca5-b327-90d703c82914](https://github.com/magesh534/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/135577936/1707abcb-487f-4c61-a0cf-738bc416509f)
![271912555-24d607e0-5123-4808-9253-58a1d8b5d80f](https://github.com/magesh534/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/135577936/bd376339-df10-489b-b05e-7005289d893e)







## Result:

Thus the program to implement the the Logistic Regression Model to Predict the Placement Status of Student is written and verified using python programming.
