# Titanic-Survival-Prediction
Machine Learning Pipeline for Titanic Survival Prediction using  Sklearn — SimpleImputer, OneHotEncoder, MinMaxScaler,  SelectKBest &amp; DecisionTree Classifier
# 🚢 Titanic Survival Prediction — ML Pipeline

A complete Machine Learning Pipeline built with Scikit-learn 
to predict passenger survival on the Titanic dataset.

## 📌 Project Overview
This project demonstrates how to build a professional 
end-to-end ML Pipeline using sklearn's Pipeline and 
ColumnTransformer to automate data preprocessing and 
model training in one clean workflow.

## 🛠️ Technologies Used
- Python 3.13
- Pandas & NumPy
- Scikit-learn (sklearn)
- Jupyter Notebook

## ⚙️ Pipeline Steps
1. **Data Loading** — Titanic train.csv dataset
2. **Feature Dropping** — Removed PassengerId, Name, 
   Ticket, Cabin
3. **Train/Test Split** — 80/20 split with random_state=42
4. **Imputation** — SimpleImputer for Age (mean) 
   and Embarked (most_frequent)
5. **Encoding** — OneHotEncoder for Sex and Embarked columns
6. **Scaling** — MinMaxScaler on all features
7. **Feature Selection** — SelectKBest with Chi2 (top 5 features)
8. **Model** — DecisionTreeClassifier

## 📊 Features Used
| Feature  | Type    | Preprocessing          |
|----------|---------|------------------------|
| Pclass   | int     | MinMaxScaler           |
| Sex      | object  | OneHotEncoder          |
| Age      | float   | SimpleImputer + Scaler |
| SibSp    | int     | MinMaxScaler           |
| Parch    | int     | MinMaxScaler           |
| Fare     | float   | MinMaxScaler           |
| Embarked | object  | Imputer + OHEncoder    |

## 🚀 How to Run
1. Clone this repository
2. Install requirements: pip install scikit-learn pandas numpy
3. Add train.csv from Kaggle Titanic dataset
4. Open Pipelines.ipynb in Jupyter Notebook
5. Run all cells from top to bottom

## 📁 Files
- Pipelines.ipynb — Main project notebook
- train.csv — Titanic training dataset (from Kaggle)

## 🎓 About
Built as part of my Machine Learning learning journey 
at Virtuali University — BBIT Program
