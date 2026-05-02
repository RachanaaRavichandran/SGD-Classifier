# SGD-Classifier
## AIM:
To write a program to predict the type of species of the Iris flower using the SGD Classifier.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1. Load Dataset
   Load the Iris dataset and separate features (X) and target labels (y).

2. Preprocess Data
   Apply **standardization** using StandardScaler to normalize the feature values.

3. Split Dataset
   Divide the data into training and testing sets using train_test_split.

4. Train Model
   Create and train the SGDClassifier using the training data.

5. Predict and Evaluate
   Predict the species using test data and calculate accuracy using accuracy_score.


## Program:
```
/*
Program to implement the prediction of iris species using SGD Classifier.

from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split
from sklearn.linear_model import SGDClassifier
from sklearn.preprocessing import StandardScaler
from sklearn.metrics import accuracy_score, classification_report

iris = load_iris()
X = iris.data
y = iris.target

scaler = StandardScaler()
X = scaler.fit_transform(X)

X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)

model = SGDClassifier(max_iter=1000, random_state=42)
model.fit(X_train, y_train)

y_pred = model.predict(X_test)

print("Accuracy:", accuracy_score(y_test, y_pred))
print("\nClassification Report:\n", classification_report(y_test, y_pred))

Developed by: Rachanaa.R
RegisterNumber:  212225040322
*/
```

## Output:
<img width="632" height="291" alt="image" src="https://github.com/user-attachments/assets/d8d70571-12bb-4cde-bb09-04531617fcad" />



## Result:
Thus, the program to implement the prediction of the Iris species using SGD Classifier is written and verified using Python programming.
