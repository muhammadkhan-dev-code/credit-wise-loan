# Credit-Wise Loan

A practical machine learning project for predicting whether a loan application should be approved or rejected using historical applicant data.

> This project aims to support faster and more consistent loan decision-making while reducing human bias and manual effort.

---

## 📌 Project Overview

Credit-Wise Loan is an end-to-end supervised learning project that uses classification models to predict loan approval outcomes. The system learns patterns from past applications and helps financial institutions make better decisions.

### Key Objectives

- Automate loan approval prediction
- Reduce manual verification effort
- Improve decision consistency
- Minimize risky approvals
- Reduce rejection of eligible applicants

---

## 🧩 Problem Statement

A financial institution receives numerous loan applications each day. Manual review can be slow and may lead to:

- Incorrect rejections of deserving applicants
- Approval of high-risk borrowers
- Inconsistent decisions across cases

This project addresses those challenges by training a predictive model on historical data.

---

## 📊 Dataset Description

The dataset contains applicant information related to demographics, income, credit behavior, employment, and loan details.

You can explore the dataset here: [Kaggle Dataset](https://www.kaggle.com/datasets/supratimnag06/loan-approval-prediction-dataset)

### Important Features

| Feature            | Description                 |
| ------------------ | --------------------------- |
| Applicant_Income   | Applicant monthly income    |
| Coapplicant_Income | Co-applicant monthly income |
| Age                | Applicant age               |
| Dependents         | Number of dependents        |
| Credit_Score       | Credit score                |
| Existing_Loans     | Existing active loans       |
| DTI_Ratio          | Debt-to-income ratio        |
| Savings            | Applicant savings           |
| Collateral_Value   | Value of collateral         |
| Loan_Amount        | Requested loan amount       |
| Loan_Term          | Loan duration               |
| Education_Level    | Education qualification     |
| Employment_Status  | Employment category         |
| Employer_Category  | Employer type               |
| Marital_Status     | Marital status              |
| Property_Area      | Rural / Semiurban / Urban   |
| Gender             | Applicant gender            |
| Loan_Purpose       | Purpose of loan             |
| Loan_Approved      | Target variable             |

---

## 🔧 Data Preprocessing

The data was carefully cleaned and transformed before model training.

### Steps Performed

- Checked and handled missing values
- Removed duplicate records where necessary
- Converted data types into appropriate formats
- Encoded categorical variables for model compatibility

### Encoding Techniques Used

#### Label Encoding

Used for ordinal categorical features such as:

- Education_Level
- Loan_Approved

#### One-Hot Encoding

Used for nominal categorical features such as:

- Employment_Status
- Marital_Status
- Loan_Purpose
- Property_Area
- Employer_Category
- Gender

The first category was dropped to avoid the dummy variable trap.

---

## 📈 Exploratory Data Analysis (EDA)

Various visualizations were created to understand the data better and identify patterns.

### Visual Insights

![Categorical feature analysis](categorical_features_analysis.png)

![Outlier detection analysis](check_for_outlier.png)

![Correlation heatmap](heatmap_image.png)

The EDA helped reveal trends related to:

- Income distribution
- Loan approval patterns
- Credit score behavior
- Correlation between numerical features
- Class balance and feature relationships

---

## 🛠️ Feature Engineering

- Encoded categorical variables
- Prepared a model-ready numeric dataset
- Removed original categorical columns after transformation

---

## ⚙️ Machine Learning Workflow

1. Data cleaning
2. Exploratory data analysis
3. Feature engineering and encoding
4. Train-test split
5. Model training
6. Prediction and evaluation

---

## 🤖 Algorithms Used

The project is designed for classification-based loan approval prediction and can be tested with models such as:

- Logistic Regression
- K-Nearest Neighbors
- Naive Bayes

---

## 📐 Evaluation Metrics

Common metrics used to measure model performance include:

- Accuracy
- Precision
- Recall
- F1 Score

### Formulas

Accuracy:

$$
Accuracy = \frac{TP + TN}{TP + TN + FP + FN}
$$

Precision:

$$
Precision = \frac{TP}{TP + FP}
$$

Recall:

$$
Recall = \frac{TP}{TP + FN}
$$

F1 Score:

$$
F1 = \frac{2 \times Precision \times Recall}{Precision + Recall}
$$

---

## 🚀 Future Improvements

- Hyperparameter tuning
- Feature selection
- Cross-validation
- Comparison of multiple classifiers
- Model deployment as a web app

---

## 👤 Author

**Muhammad Khan**

Machine Learning Enthusiast

---

If you found this project useful, consider giving it a star.
