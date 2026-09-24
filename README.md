# 🏦 Loan Approval Prediction

## 📌 Project Overview

This project uses machine learning classification algorithms to predict
whether a loan application will be approved based on applicant and
loan-related features.

The project demonstrates a complete machine learning workflow including
data preprocessing, exploratory data analysis, feature encoding,
feature scaling, model training, evaluation, and feature engineering.

---

## 🎯 Objective

The objective of this project is to build a machine learning model that
can predict loan approval based on the available applicant information.

---

## 📊 Dataset

The dataset contains information related to loan applicants, including
features such as:

- Applicant Income
- Coapplicant Income
- Credit Score
- DTI Ratio
- Savings
- Education Level
- Employment Status
- Marital Status
- Loan Purpose
- Property Area
- Gender
- Employer Category

### Target Variable

`Loan_Approved`

The target represents whether the loan application was approved.

---

## 🔧 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 🛠️ Machine Learning Workflow

### 1. Data Loading

The dataset is loaded using Pandas.

### 2. Data Preprocessing

The following preprocessing steps were performed:

- Identification of numerical and categorical columns
- Missing-value imputation
- Removal of `Applicant_ID`
- Label encoding
- One-hot encoding

### 3. Exploratory Data Analysis

EDA was performed to understand:

- Loan approval distribution
- Education-level distribution
- Applicant income
- Coapplicant income
- Credit score
- Outliers
- Relationship between features and loan approval

### 4. Correlation Analysis

A correlation heatmap was used to examine relationships between
numerical variables.

### 5. Train-Test Split

The dataset was divided into training and testing sets using an
80/20 split.

### 6. Feature Scaling

StandardScaler was applied to scale the features before model training.


## Visualization
<div align="center">

<img src="https://github.com/user-attachments/assets/fcf83ba2-fcef-4970-9228-077a27f143d6" width="500" height="350" />

<img src="https://github.com/user-attachments/assets/a3c0896d-b192-4801-857f-87bebe51bd1d" width="500" height="350" />

<img src="https://github.com/user-attachments/assets/04f2fc16-f2d7-4e26-a8b6-7c3b6e2b4a60" width="500" height="350" />

<img src="https://github.com/user-attachments/assets/20e6be6b-ff6c-44a8-b9f8-536194aa3097" width="500" height="350" />

<img src="https://github.com/user-attachments/assets/e7b4335e-11b2-472a-bc7c-09c91ffb99a7" width="500" height="350" />

<img src="https://github.com/user-attachments/assets/575c7b82-7861-4d9a-8bc3-70c39c71ff9d" width="500" height="350" />

<img src="https://github.com/user-attachments/assets/92616ae5-64da-45d5-bc9b-2f15eb604979" width="500" height="350" />

<img src="https://github.com/user-attachments/assets/def7c25a-7847-4f33-9585-f056902c3d75" width="500" height="350" />

</div>


---

## 🤖 Models Used

The following classification algorithms were evaluated:

### Logistic Regression

Used as a baseline classification model.

### K-Nearest Neighbors

A distance-based classification algorithm.

### Naive Bayes

A probabilistic classification algorithm based on Bayes' theorem.

---

## 📈 Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

| Model | Accuracy | Precision | Recall | F1 Score |
|------|----------|-----------|--------|----------|
| Logistic Regression | 0.865 | 0.78 | 0.770 | 0.776 |
| KNN | 0.79 | 0.73 | 0.49 | 0.58 |
| Naive Bayes | 0.865 | 0.80 | 0.73 | 0.76 |

> Replace `XX` with the actual values from the notebook.

---

## 🧪 Feature Engineering

Additional features were created by applying squared transformations
to:

- `DTI_Ratio`
- `Credit_Score`

The models were then retrained to investigate whether the engineered
features improved performance.

---

## 📊 Results

The performance before and after feature engineering can be compared
using the evaluation metrics.

| Model | Before FE | After FE |
|------|-----------|----------|
| Logistic Regression | Accuracy:0.86 | Accuracy:0.86 |
| KNN | Accuracy:0.79 | Accuracy:0.76 |
| Naive Bayes | Accuracy:0.86 | Accuracy:0.86 |

---

## 📁 Project Structure

```text
loan-approval-prediction/
│
├── data/
│   └── loan_approval_data.csv
│
├── notebooks/
│   └── loan_approval_prediction.ipynb
│
├── README.md
