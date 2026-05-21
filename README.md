# SGD-Regressor-for-Multivariate-Linear-Regression

## AIM:
To write a program to predict the price of the house and number of occupants in the house with SGD regressor.

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
Program to implement the multivariate linear regression model for predicting the price of the house and number of occupants in the house with SGD regressor.
Developed by: KARTHEESHWAR D J
RegisterNumber:  212225040173
*/
import numpy as np
X = np.array([
    [2, 80, 50],
    [3, 60, 40],
    [5, 90, 70],
    [7, 85, 80],
    [9, 95, 90]
], dtype=float)
y = np.array([50, 45, 70, 80, 95], dtype=float)
w = np.zeros(X.shape[1])
b = 0
lr = 0.0001
epochs = 1000
for epoch in range(epochs):
    for i in range(len(X)):
        y_pred = np.dot(X[i], w) + b
        error = y_pred - y[i]
        w = w - lr * error * X[i]
        b = b - lr * error
print("Weights:", w)
print("Bias:", b)
predictions = np.dot(X, w) + b
print("\nPredictions:")
print(predictions)
```

## Output:
<img width="612" height="125" alt="image" src="https://github.com/user-attachments/assets/b27b55a0-a1a1-41e0-a555-b3e0a47d781e" />
<img width="1292" height="511" alt="image" src="https://github.com/user-attachments/assets/c5f8b567-d448-4e64-89c3-9377cefae9e5" />

## Result:
Thus the program to implement the multivariate linear regression model for predicting the price of the house and number of occupants in the house with SGD regressor is written and verified using python programming.
