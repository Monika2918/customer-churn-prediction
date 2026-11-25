# Customer Churn Prediction

## About the Project

This project is about predicting customer churn using Python and Machine Learning.

Customer churn means when a customer stops using a company's services. In this project, I used the Telco Customer Churn dataset to understand customer behaviour and identify patterns that may be related to churn.

## Objectives

- Understand customer data through analysis.
- Clean and prepare the dataset.
- Find patterns related to customer churn.
- Build machine learning models.
- Compare model performance.
- Predict whether a customer is likely to leave.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Dataset

I used the IBM Telco Customer Churn dataset.

It contains information about customers, including:
- Gender and senior citizen status
- Tenure
- Monthly and total charges
- Contract type
- Internet services
- Churn status

## Work Done

1. Loaded and explored the dataset.
2. Checked missing values and duplicate records.
3. Cleaned the TotalCharges column.
4. Removed the customer ID column.
5. Converted categorical columns into numerical values.
6. Split the data into training and testing sets.
7. Applied feature scaling.
8. Trained different machine learning models.
9. Compared model performance.
10. Tried different classification thresholds.
11. Handled class imbalance using class weights.
12. Analyzed feature importance.

## Models Used

- Logistic Regression
- Decision Tree
- Random Forest
- Logistic Regression with threshold tuning
- Logistic Regression with balanced class weights

## Model Results

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 80.38% | 64.76% | 57.49% | 60.91% |
| Logistic Regression (Threshold 0.3) | 74.34% | 51.17% | 75.94% | 61.14% |
| Decision Tree | 71.64% | 46.61% | 45.99% | 46.30% |
| Random Forest | 78.82% | 62.34% | 51.34% | 56.31% |
| Weighted Logistic Regression | 72.64% | 49.09% | 79.68% | 60.75% |

## Some Observations

- Customers with month-to-month contracts had a higher churn rate.
- Customers with shorter tenure were more likely to churn.
- Customers who churned had higher average monthly charges.
- Changing the classification threshold increased churn recall.
- Class weighting also helped identify more churn customers.

## Project Structure

```text
customer-churn-prediction/
│
├── data/
├── models/
├── notebooks/
├── src/
├── visualizations/
├── .gitignore
└── README.md
```

## How to Run

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open `notebooks/Customer_Churn_Prediction.ipynb` and run the cells.

## Conclusion

Through this project, I learned how to work with customer data, perform data preprocessing, train machine learning models and evaluate their performance.

I also understood the importance of precision, recall and F1 score when working with imbalanced datasets.

**Project Status:** Completed
