# Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student


## AIM:
To write a program to implement the the Logistic Regression Model to Predict the Placement Status of Student.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
```
```
1. 1.Import the required packages and print the present data.

2.Print the placement data and salary data.

3.Find the null and duplicate values.

4.Using logistic regression find the predicted values of accuracy , confusion matrices.

5.Display the results.
```
``` 

## Program:
```
``
/*
Program to implement the the Logistic Regression Model to Predict the Placement Status of Student.
Developed by: anumitha.M.R
RegisterNumber: 21223040018 
*/
```
```
data = pd.read_csv("/content/Placement_Data.csv")
data.head()
data1=data.copy()
data1=data1.drop(["sl_no","salary"],axis=1)
data1.head()
data1.isnull().sum()
data1.duplicated().sum()
x=data1.iloc[:,:-1]
x
y=data1["status"]
y
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)
from sklearn.metrics import accuracy_score
accuracy = accuracy_score(y_test,y_pred)
accuracy
from sklearn.metrics import confusion_matrix
confusion = (y_test,y_pred)
confusion
from sklearn.metrics import classification_report
classification_report1 = classification_report(y_test,y_pred)
print(classification_report1)
lr.predict([[1,80,1,90,1,1,90,1,0,85,1,85]])
````
````
```
````
## Output:
````
````
![image](https://github.com/anumitha2005/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/155522855/ef1e4258-da36-4966-b1cc-9953752c717f)

![image](https://github.com/anumitha2005/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/155522855/61778765-87a6-4937-9793-748a0880c61a)
![image](https://github.com/anumitha2005/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/155522855/5c58b461-634b-41c4-a323-a28832302e50)
![image](https://github.com/anumitha2005/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/155522855/42c0e8e9-07bd-4f03-8d33-0e89a64c2979)
![image](https://github.com/anumitha2005/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/155522855/aa59a738-501c-49af-ac56-85d3736d59b2)
![image](https://github.com/anumitha2005/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/155522855/8353e12e-26be-4e5c-9cae-d6d900ba3d0f)
![image](https://github.com/anumitha2005/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/155522855/c2fe54ce-2cdb-42c7-af30-42362c942fd7)
![image](https://github.com/anumitha2005/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/155522855/153eb253-2834-466b-ad05-09fe07aab92c)
![image](https://github.com/anumitha2005/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/155522855/9049601e-c554-4e0d-ab6c-73a017643b2b)
![image](https://github.com/anumitha2005/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/155522855/461ae515-ee20-4d34-9e44-e7475208ce6c)
![image](https://github.com/anumitha2005/Implementation-of-Logistic-Regression-Model-to-Predict-the-Placement-Status-of-Student/assets/155522855/a761d06f-00ed-48fa-a5ab-20ad12a967ff)

````
````




## Result:
Thus the program to implement the the Logistic Regression Model to Predict the Placement Status of Student is written and verified using python programming.
