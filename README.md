# 🚢 Titanic Survival Prediction - Machine Learning Project

## 📌 Project Overview
This project aims to develop a machine learning model that predicts whether a passenger survived the Titanic disaster based on attributes like age, gender, ticket class, fare, and more. The goal is to build a reliable classification model that can analyze survival likelihood.

---

## 📂 Dataset Description
The dataset contains information about passengers on the Titanic, including:

| Column       | Description                                  |
|--------------|----------------------------------------------|
| Survived     | 0 = No, 1 = Yes                              |
| Pclass       | Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd)  |
| Sex          | Male or Female                               |
| Age          | Age of passenger                             |
| SibSp        | # of siblings / spouses aboard               |
| Parch        | # of parents / children aboard               |
| Fare         | Ticket fare                                  |
| Embarked     | Port of Embarkation (S, C, Q)                |

---

## 🧼 Data Preprocessing
- Handled missing values:
  - Filled missing `Age` values with mean
  - Filled missing `Fare` values with mode
- Categorical Encoding:
  - Converted `Sex` and `Embarked` using One-Hot Encoding (`get_dummies`)
- Normalization:
  - Applied **MinMaxScaler** to `Age` and `Fare` columns

---

## 🧠 Model Used
- **Logistic Regression** from scikit-learn
- Input features selected: `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked`
- Train-test split used for model training and validation

---

## 📊 Model Evaluation

- **Accuracy**: 1.00  
- **Confusion Matrix**:
