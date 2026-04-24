# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

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
# Step 1: Import Libraries
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error, r2_score

# Step 2: Create Dataset (Hours Studied vs Marks Scored)
data = {
    "Hours_Studied": [1,2,3,4,5,6,7,8,9,10],
    "Marks_Scored": [35,40,50,55,60,65,70,80,85,95]
}

df = pd.DataFrame(data)

# Display Dataset
print("Dataset:")
print(df)

# Step 3: Split Features (X) and Target (Y)
X = df[["Hours_Studied"]]   # Independent Variable
y = df["Marks_Scored"]      # Dependent Variable

# Step 4: Split Data into Training and Testing
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)

# Step 5: Train Simple Linear Regression Model
model = LinearRegression()
model.fit(X_train, y_train)

# Step 6: Predict Test Data
y_pred = model.predict(X_test)

# Step 7: Evaluate Model
print("\nModel Parameters")
print("Intercept:", model.intercept_)
print("Slope:", model.coef_[0])

print("\nPerformance Metrics")
print("Mean Squared Error:", mean_squared_error(y_test, y_pred))
print("R2 Score:", r2_score(y_test, y_pred))

# Step 8: Visualize Regression Line
plt.figure(figsize=(8,6))
plt.scatter(X, y, color="blue", label="Actual Data")
plt.plot(X, model.predict(X), color="red", label="Regression Line")
plt.xlabel("Hours Studied")
plt.ylabel("Marks Scored")
plt.title("Simple Linear Regression")
plt.legend()
plt.show()

# Step 9: Predict Marks for New Input
hours = 7.5
predicted_marks = model.predict([[hours]])
print("\nPredicted Marks for", hours, "hours =", predicted_marks[0])

Developed by: Megala M S
RegisterNumber:  212225040230
*/
```

## Output:
<img width="383" height="271" alt="Screenshot 2026-04-24 141147" src="https://github.com/user-attachments/assets/f4aea7e3-73e9-416b-9342-3f1434bc0623" />
<img width="1054" height="822" alt="Screenshot 2026-04-24 141134" src="https://github.com/user-attachments/assets/f14bc3c9-9616-4b1b-993d-6e7fdb8b9cab" />


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
