# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required packages.
2.Import the dataset to operate on.
3.Split the dataset.
4.Predict the required output.
5.End the program.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: JANANI R
RegisterNumber:  212221230039

import pandas as pd
data=pd.read_csv("/content/spam.csv",encoding='Windows-1252')
import chardet
file='spam.csv'
with open(file,'rb') as rawdata:
	result =chardet.detect(rawdata.read(100000))
result
data.head()
data.info()
data.isnull().sum()
x=data["v1"].values
y=data["v2"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.feature_extraction.text import CountVectorizer
cv=CountVectorizer()
x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)
from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred
*/
```

## Output:
![SVM For Spam Mail Detection](sam.png)
![Screenshot 2022-11-30 112540](https://user-images.githubusercontent.com/94288340/204719017-ffb7f2fa-4fb1-40b8-8f7c-3623db9c1d84.png)
![Screenshot 2022-11-30 112617](https://user-images.githubusercontent.com/94288340/204719053-2b5864bb-afc1-4ea4-b68d-8e97a6756f99.png)
![Screenshot 2022-11-30 112652](https://user-images.githubusercontent.com/94288340/204719112-4eb7dc95-2cee-4ecc-a602-1e7272abf9e6.png)

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
