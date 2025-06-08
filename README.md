# 🔁 Customer Churn Prediction with Logistic Regression

A classification project using **Logistic Regression** to predict customer churn based on demographics, service usage, and contract information. This project utilizes a real-world dataset from Kaggle and is implemented in Python using the `scikit-learn` library.

---

## 📁 Project Structure

```

customer-churn-logistic-regression/
│
├── Logistic_Regression_Churn.ipynb # Jupyter notebook with complete code and analysis
├── churn_data.csv # Cleaned dataset (from Kaggle - loaded in Kaggle environment)
├── README.md # Project documentation (this file)├── sentiment-analysis.ipynb
├── README.md
├── LICENSE
└── sentiment_dataset.csv
```
---

## 🎯 Project Objectives

- Understand the **logistic regression** algorithm for binary classification  
- Train a model to predict if a customer is likely to **churn**  
- Perform **data cleaning**, **encoding**, and **feature scaling**  
- Evaluate performance using metrics like **accuracy**, **confusion matrix**, and **classification report**  
- Visualize churn predictions and feature importance

---

## 🔍 Dataset Overview

Dataset used:  
👉 [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

**Key Features Used:**

| Feature               | Description                                 |
|-----------------------|---------------------------------------------|
| `Monthly Charges`     | Monthly fee paid by the customer            |
| `Total Charges`       | Total amount billed                         |
| `Tenure Months`       | Number of months as a customer              |
| `Contract`            | Contract type (Month-to-month, etc.)        |
| `Internet Service`    | Type of internet service                    |
| `Payment Method`      | Billing method                              |
| `Tech Support`        | Whether tech support is subscribed          |

**Target Variable:** `Churn Value` (0 = No Churn, 1 = Churn)

---

## 🧠 Modeling Steps

1. **Load Data**  
   Use `pandas` to load the dataset and inspect structure.

2. **Preprocess Data**  
   - Drop irrelevant columns (`Count`, `Lat Long`, etc.)  
   - Convert categorical variables using **Label Encoding**  
   - Handle missing values and convert `Total Charges` to numeric

3. **Split the Data**  
   Split into training and testing sets (80/20 split).

4. **Train the Model**  
   Fit a logistic regression model using `scikit-learn`.

5. **Evaluate the Model**  
   - Generate predictions  
   - Display **confusion matrix**, **classification report**, and **accuracy**  
   - Visualize churn vs no churn

---

## 📊 Sample Output

Accuracy: 80.32%
Precision (Churn): 0.74
Recall (Churn): 0.66
F1 Score: 0.70
