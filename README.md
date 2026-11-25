# customer-churn-prediction

A Machine Learning project that analyzes customer data and predicts whether a customer is likely to leave a telecommunications service.

## 1. Project Overview

Customer churn occurs when customers stop using a company's services.

The goal of this project is to analyze customer behavior, identify patterns associated with churn, and build machine learning classification models to predict customer churn.

## 2. Objectives

- Analyze customer data to identify churn patterns.
- Perform data cleaning and preprocessing.
- Explore relationships between customer features and churn.
- Build and compare multiple machine learning models.
- Evaluate models using accuracy, precision, recall, and F1-score.
- Explore threshold tuning and class balancing.

## 3. Dataset

**Dataset:** IBM Telco Customer Churn

The dataset contains customer information such as:
- Customer demographics
- Tenure
- Monthly charges
- Total charges
- Contract type
- Internet and additional services
- Churn status

## 4. Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- GitHub

## 5. Project Workflow

1. Data loading and exploration
2. Exploratory Data Analysis (EDA)
3. Data cleaning and preprocessing
4. Categorical encoding
5. Train-test splitting
6. Feature scaling
7. Model training
8. Model evaluation
9. Threshold tuning
10. Class imbalance handling
11. Feature importance analysis
12. Customer churn prediction

## 6. Machine Learning Models

The following approaches were evaluated:

- Logistic Regression
- Decision Tree
- Random Forest
- Logistic Regression with a modified classification threshold
- Logistic Regression with balanced class weights

## 7. Model Comparison

| Model / Approach | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| Logistic Regression (0.5) | 80.38% | 64.76% | 57.49% | 60.91% |
| Logistic Regression (0.3) | 74.34% | 51.17% | 75.94% | 61.14% |
| Decision Tree | 71.64% | 46.61% | 45.99% | 46.30% |
| Random Forest | 78.82% | 62.34% | 51.34% | 56.31% |
| Weighted Logistic Regression | 72.64% | 49.09% | 79.68% | 60.75% |

## 8. Key Findings

- Customers with month-to-month contracts showed a higher churn rate.
- Customers who churned had lower average tenure.
- Customers who churned had higher average monthly charges.
- Lowering the classification threshold increased churn recall.
- Using balanced class weights improved the model's ability to identify churn customers.
- Tenure, TotalCharges, and MonthlyCharges were among the most important features in the Random Forest model.

## 9. Visualizations

The project includes visual analysis of customer churn and a feature importance visualization.

Feature importance chart:

`visualizations/feature_importance.png`

## 10. Project Structure

```text
customer-churn-prediction/
│
├── data/
├── models/
├── notebooks/
│   └── Customer_Churn_Prediction.ipynb
│
├── src/
├── visualizations/
│   └── feature_importance.png
│
├── .gitignore
└── README.md
```

## 11. How to Run

1. Clone or download this repository.
2. Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

3. Open Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `notebooks/Customer_Churn_Prediction.ipynb`.
5. Run the notebook cells in order.

## 12. Conclusion

This project demonstrates an end-to-end customer churn prediction workflow using Python and machine learning.

It also explores why accuracy alone is not sufficient for evaluating an imbalanced classification problem and how threshold tuning and class weighting can improve churn detection.

## 13. Future Improvements

- Hyperparameter tuning
- Cross-validation
- Model deployment using Streamlit
- More advanced churn prediction models

---

**Project Type:** Machine Learning / Classification  
**Language:** Python  
**Status:** Completed
