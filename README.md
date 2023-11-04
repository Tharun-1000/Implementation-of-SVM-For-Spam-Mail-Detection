# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the necessary python packages using import statements.

2.Read the given csv file usingread_csv() method and print the number of contents to be displayed using df.head().

3.Split thedataset using train_test_split.

4.Calculate Y_Pred and accuracy. 

5.Print all the outputs.

6.End the Program.


## Program:

/*
Program to implement the SVM For Spam Mail Detection..
Developed by: THARUN K

RegisterNumber: 212222040172

import pandas as pd
data=pd.read_csv("spam.csv",encoding='latin-1')
import chardet
file='/content/spam.csv'
with open(file,'rb') as rawdata:
result = chardet.detect(rawdata.read(100000))
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
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy


*/


## Output:

RESULT OUTPUT:

![image](https://github.com/Tharun-1000/Implementation-of-SVM-For-Spam-Mail-Detection/assets/135952958/987092de-19f4-4c11-b4ef-b4e623a72354)

data.head():

![image](https://github.com/Tharun-1000/Implementation-of-SVM-For-Spam-Mail-Detection/assets/135952958/9e34711b-db47-4e2e-acb3-990e4647bcdd)

data.info():

![image](https://github.com/Tharun-1000/Implementation-of-SVM-For-Spam-Mail-Detection/assets/135952958/5e3e6ea9-23aa-4022-bc28-45ee12019b07)

data.isnull().sum():

![image](https://github.com/Tharun-1000/Implementation-of-SVM-For-Spam-Mail-Detection/assets/135952958/2b1fe3c8-e6ae-4c42-aa6c-45783646feb9)

Y_prediction VALUE:

![image](https://github.com/Tharun-1000/Implementation-of-SVM-For-Spam-Mail-Detection/assets/135952958/4d167129-a6b7-405d-9a95-5237d56e6f94)

ACCURACY VALUE:

![image](https://github.com/Tharun-1000/Implementation-of-SVM-For-Spam-Mail-Detection/assets/135952958/ae35226e-d69a-4bb2-af3d-92b3375bbf3a)




## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
