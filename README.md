# 🚗 Electric Vehicle Purchase Prediction

## 📌 Project Overview

This project predicts whether a customer is likely to purchase an Electric Vehicle (EV) using machine learning.

The project was developed as part of the **Kaggle Playground Series – Season 6 Episode 9: Predicting Electric Vehicle Purchases** competition.

## 🎯 Problem Statement

The goal is to predict the probability that a customer will purchase an electric vehicle based on demographic, financial, commuting, charging infrastructure, environmental concern, and other factors.

This is a **Binary Classification** problem.

### Target Variable

`Will_Buy_EV`

* `0` → No
* `1` → Yes

## 📊 Dataset

The dataset contains information such as:

* Age
* Annual Income
* Daily Commute Distance
* Number of Cars Owned
* Charging Stations Near Home
* Charging Stations Near Work
* Environmental Concern Level
* Gender
* City Type
* Current Car Type
* Home Charging Possibility
* Subsidy Availability
* Range Anxiety Level

## 🔍 Exploratory Data Analysis

Key observations from the analysis:

* Customers with subsidies showed a higher EV purchase rate.
* Customers with higher environmental concern were more likely to purchase an EV.
* Home charging availability showed an association with EV purchase intention.
* Annual income was somewhat higher among customers who purchased/were predicted to purchase EVs.

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

* Removed the `id` column from model features.
* Converted the target variable from `Yes/No` to `1/0`.
* Split the training data into training and validation sets.
* Used **One-Hot Encoding** for categorical variables.
* Kept numerical variables in their original form.

## 🤖 Models

### Logistic Regression

Validation ROC-AUC:

**0.9085**

### XGBoost Classifier

Initial validation ROC-AUC:

**0.9417**

After hyperparameter tuning:

**Best Validation ROC-AUC: 0.941755**

## 🏆 Kaggle Result

**Kaggle ROC-AUC: 0.94155**

The final predictions were generated using the tuned XGBoost model and submitted to Kaggle.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Matplotlib
* Jupyter Notebook / Google Colab
* Kaggle

## 📁 Project Structure

```text
EV-Purchase-Prediction/
│
├── EV_Purchase_Prediction.ipynb
├── submission.csv
└── README.md
```

## 📈 Evaluation Metric

The competition uses **ROC-AUC (Area Under the Receiver Operating Characteristic Curve)** to evaluate model performance.

## 👩‍💻 Author

**Geeta Bamhane**

MSc Data Science | Aspiring AI/ML Engineer & Data Scientist
