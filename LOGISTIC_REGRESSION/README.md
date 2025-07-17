# 🚢 Titanic - Machine Learning from Disaster

This project explores survival prediction on the Titanic dataset using logistic regression. It includes data preprocessing, feature engineering, EDA, model training, and hyperparameter tuning.

---

## 📂 Project Overview

The goal is to predict which passengers survived the Titanic shipwreck based on features like age, gender, class, and family connections. This is a classic binary classification problem.

---

## 🛠️ Tech Stack & Libraries

- Python 🐍
- Pandas & NumPy 📊
- Matplotlib & Seaborn 📈
- Scikit-learn 🤖
- Jupyter Notebook 📒

---

## 🔍 Exploratory Data Analysis (EDA)

- Checked for null values and missing data
- Visualized distributions (Survival rate, Age, Fare)
- Analyzed correlation heatmap
- Investigated relationships between features like `Sex`, `Pclass`, and `Survived`

---

## 🧠 Feature Engineering

- **FamilySize**: `SibSp` + `Parch` + 1
- **IsAlone**: Binary flag based on `FamilySize`
- Handled missing values:
  - `Age` filled with **median**
  - `Embarked` filled with **mode**
  - `Fare` filled with **median**

---

## 📊 Feature Selection

Selected features based on correlation, importance, and business understanding:

- `Age`, `Fare`, `Sex`, `Pclass`, `Embarked`, `FamilySize`, `IsAlone`

Removed highly correlated or irrelevant features to reduce noise and avoid multicollinearity.

---

## 🤖 Model Training

- Model used: **Logistic Regression**
- Preprocessing pipeline created with:
  - `StandardScaler` for numerical data
  - `OneHotEncoder` for categorical data
  - `SimpleImputer` for handling missing values

---

## 🛠️ Hyperparameter Tuning

- Used **GridSearchCV** with **StratifiedKFold**
- Tuned parameters like:
  - `C` (regularization strength)
  - `penalty` (`l1`, `l2`)
  - `solver` (`liblinear`, `saga`, etc.)

---

## 🧪 Model Evaluation

- Accuracy Score
- Classification Report (Precision, Recall, F1)
- Confusion Matrix

---

## ✅ Final Output

- Achieved model accuracy in the ~80% range on test data.
- Final model used to make predictions on unseen data (test set from Kaggle).

---


