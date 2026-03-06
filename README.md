# Data Pipeline Development for Customer Churn Prediction

## Internship Task

This project was completed as part of the **CodTech Data Science Internship – Task 1**.

The objective of this task was to build a **data pipeline for preprocessing, transformation, and model training** using Python libraries such as **Pandas** and **Scikit-learn**.

---

## Project Overview

Customer churn prediction is an important problem for telecom companies.
The goal of this project is to prepare customer data using an automated **ETL pipeline** and train a machine learning model to predict whether a customer is likely to churn.

---

## Dataset

The project uses the **Telco Customer Churn dataset**, which contains information about telecom customers including:

* Demographic information
* Account information
* Services subscribed
* Billing details
* Churn status

Dataset features include:

* `tenure`
* `MonthlyCharges`
* `TotalCharges`
* `InternetService`
* `Contract`
* `PaymentMethod`
* `Churn` (Target variable)

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Seaborn
* Matplotlib
* Joblib

---

## Project Workflow

### 1. Data Loading

The dataset was loaded using **Pandas** and inspected for structure and data types.

### 2. Data Cleaning

* Converted `TotalCharges` column to numeric values
* Handled missing values
* Removed unnecessary columns such as `customerID`

### 3. Data Preprocessing

* Numerical features were scaled using **StandardScaler**
* Categorical features were encoded using **OneHotEncoder**

### 4. Pipeline Creation

A **Scikit-learn Pipeline** was created to automate preprocessing and model training.

Pipeline steps:

1. ColumnTransformer
2. Feature scaling
3. One-hot encoding
4. Logistic Regression model

### 5. Model Training

The dataset was split into training and testing sets using **train_test_split**.

A **Logistic Regression model** was trained using the pipeline.

### 6. Model Evaluation

The model performance was evaluated using:

* Accuracy Score
* Classification Report
* Confusion Matrix

### 7. Model Saving

The trained pipeline model was saved using **Joblib** for future use.

---

## Project Structure

```
        ├── customer-churn-project-data-churn.csv
        ├── task1_pipeline.ipynb
        ├── churn_pipeline_model.pkl
        └── README.md
```

---

## Output

The project successfully created an automated pipeline that:

* Preprocesses the dataset
* Transforms features
* Trains a machine learning model
* Generates predictions for customer churn

---

## Author

**Anjali J.**
Data Science Intern – CodTech
