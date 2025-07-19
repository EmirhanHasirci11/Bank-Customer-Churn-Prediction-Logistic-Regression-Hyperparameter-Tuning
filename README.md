# 🏦 Bank Customer Churn Prediction - Logistic Regression & Hyperparameter Tuning

This notebook demonstrates a **Logistic Regression** model applied to a scaled dataset of bank customers. The focus is not only on training the model, but also on understanding the difference between **GridSearchCV** and **RandomizedSearchCV** for hyperparameter optimization.

---

## 🎯 Objective

- Predict customer subscription behavior (`subscribed`) using logistic regression.
- Apply **Grid Search** and **Randomized Search** to optimize the model.
- Compare performance in terms of accuracy and runtime.
- Use a **scaled, ready-to-use dataset** with all preprocessing completed.

---

## 📁 Dataset Overview

The dataset consists of customer-related features that have been **scaled and cleaned**, allowing direct use in ML models.

| Feature Name                 | Description                                                  |
|-----------------------------|--------------------------------------------------------------|
| `age`                       | Age of the customer                                          |
| `job_satisfaction`          | Satisfaction level (Likert scale, e.g., 1–10)                |
| `balance`                   | Account balance (in monetary units)                          |
| `duration_last_call`        | Duration of the last contact (in seconds)                    |
| `num_contacts_last_month`   | Number of contacts in the previous month                     |
| `has_housing_loan`          | Whether the customer has a housing loan (1 = Yes, 0 = No)    |
| `has_personal_loan`         | Whether the customer has a personal loan (1 = Yes, 0 = No)   |
| `communication_type`        | Encoded type of communication used (e.g., call, email)       |
| `days_since_last_contact`   | Number of days passed since the last contact                 |
| `campaign_response_score`   | Internal score representing response likelihood              |
| `subscribed`                | Target variable (1 = Subscribed, 0 = Not Subscribed)         |

---

## ⚙️ Key Steps in the Notebook

### 1. **Data Overview**
- Preview of feature distributions
- Confirm dataset shape and readiness for modeling

### 2. **Model Training**
- Split data into training and testing sets
- Fit a **Logistic Regression** model
- Evaluate using classification metrics (accuracy, precision, recall, F1)

### 3. **Hyperparameter Tuning**
#### ✅ GridSearchCV
- Exhaustive parameter search
- Best performance but time-intensive

#### 🎲 RandomizedSearchCV
- Faster but randomized search
- Good performance with reduced runtime

### 4. **Comparison**
- Accuracy, confusion matrix, and classification report
- Interpretation of results from both search strategies

---

## 📈 Visuals Included
- Confusion matrix heatmap
- Accuracy score comparison
- Classification report output
