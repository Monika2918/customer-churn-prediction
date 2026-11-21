# Customer Churn Prediction

---

## 1. PROJECT OVERVIEW

Customer Churn Prediction is a Machine Learning project that aims to identify customers who are likely to stop using a company's services.

Customer churn is an important business problem because retaining existing customers can help businesses reduce losses and improve customer satisfaction.

This project uses customer information and service-related data to build a classification model that predicts whether a customer will churn.

## 2. PROJECT OBJECTIVES

- Understand customer behaviour using Exploratory Data Analysis (EDA).
- Clean and preprocess the dataset.
- Identify factors that may influence customer churn.
- Perform feature engineering.
- Build and train Machine Learning classification models.
- Evaluate and compare model performance.
- Improve the model where necessary.
- Develop a simple customer churn prediction system.
- Document the complete project and publish it on GitHub.

## 3. DATASET INFORMATION

- **Dataset:** IBM Telco Customer Churn Dataset
- **Original file:** `WA_Fn-UseC_-Telco-Customer-Churn.csv`
- **Total original records:** 7,043
- **Original columns:** 21
- **Target variable:** `Churn`

### Dataset Features

- Customer demographics
- Customer tenure
- Internet and phone services
- Contract information
- Payment methods
- Monthly charges
- Total charges
- Customer churn status

### Target Variable

- `No` = Customer did not leave.
- `Yes` = Customer left.

## 4. TECHNOLOGIES AND LIBRARIES

### Programming Language
- Python

### Development Environment
- Jupyter Notebook

### Python Libraries
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical visualization
- **Scikit-learn** – Machine Learning and model evaluation

### Version Control
- Git and GitHub

## 5. PROJECT WORKFLOW – 10 DAYS

### DAY 1: PROJECT SETUP AND DATASET COLLECTION

- Create the project repository on GitHub.
- Set up the local project folder structure.
- Install and verify the required Python libraries.
- Download and extract the dataset.
- Load the dataset using Pandas.
- Inspect the first few records.

### DAY 2: EXPLORATORY DATA ANALYSIS (EDA)

- Understand the dataset structure using `shape`, `head()` and `info()`.
- Generate descriptive statistics.
- Identify missing values.
- Study the distribution of the target variable.
- Analyze customer churn by contract type.
- Analyze customer tenure and monthly charges.
- Create visualizations to understand customer behaviour.
- Identify patterns associated with churn.

### DAY 3: DATA CLEANING AND PREPROCESSING

- Create a working copy of the original dataset.
- Convert `TotalCharges` into a numerical data type.
- Identify and handle missing values.
- Check for duplicate records.
- Remove the unnecessary `customerID` column.
- Separate input features and target variable.
- Convert the target variable into numerical labels.
- Apply One-Hot Encoding to categorical features.
- Save the processed feature and target datasets.
- - Removed 11 records with missing TotalCharges values.

### DAY 4: FEATURE ENGINEERING AND DATA PREPARATION

- Reviewed the processed input features.
- Loaded the processed feature and target datasets.
- Split the dataset into training and testing sets.
- Used stratified sampling to maintain class distribution.
- Applied StandardScaler for feature scaling.
- Transformed training and testing features.
- Verified the scaled feature values.

### DAY 5: FIRST MACHINE LEARNING MODEL – LOGISTIC REGRESSION

- Understood supervised learning and classification.
- Created a Logistic Regression model using Scikit-learn.
- Trained the model using training data.
- Generated predictions on test data.
- Compared actual and predicted values.
- Evaluated the model using accuracy score.
- Achieved an initial test accuracy of 80.38%.
- Understood the importance of feature scaling.

### DAY 6: ADDITIONAL MACHINE LEARNING MODELS

- Understand Decision Tree classification.
- Train a Decision Tree model.
- Understand Random Forest classification.
- Train a Random Forest model.
- Generate predictions using both models.
- Compare their initial performance.

### DAY 7: MODEL EVALUATION AND COMPARISON

Evaluate model performance using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC-AUC score

Additional activities:

- Compare the trained models.
- Understand false positives and false negatives.
- Identify the most suitable model based on evaluation results.

### DAY 8: MODEL IMPROVEMENT

- Study the class imbalance in the dataset.
- Explore suitable techniques for handling class imbalance.
- Experiment with model hyperparameters.
- Apply appropriate model improvement techniques.
- Compare improved models with their initial versions.
- Select a model based on evaluation results.

### DAY 9: PREDICTION SYSTEM AND VISUALIZATIONS

- Prepare the selected model for predictions.
- Build a simple customer churn prediction interface.
- Accept customer details as input.
- Predict whether a customer is likely to churn.
- Display the prediction result.
- Create useful visualizations to explain model insights.

### DAY 10: FINAL DOCUMENTATION AND GITHUB

- Organize the project files and folders.
- Save the final trained model.
- Complete the project README.
- Document the methodology and results.
- Add relevant visualizations.
- Upload the final notebooks, code and required files to GitHub.
- Review the complete project.
- Prepare an explanation for interviews and portfolio presentations.

## 6. DATA PREPROCESSING SUMMARY

The preprocessing workflow includes:

- Handling missing values in `TotalCharges`.
- Removing the `customerID` identifier.
- Converting categorical variables into numerical features.
- Encoding the target variable.
- Preparing separate feature and target datasets.

### Processed Dataset Details

| Description | Value |
|---|---:|
| Customer records | 7,032 |
| Input features | 30 |
| Target variable | Churn |
| No churn | 0 |
| Churn | 1 |

## 7. PROJECT FOLDER STRUCTURE

```text
customer-churn-prediction/
│
├── data/
│   ├── WA_Fn-UseC_-Telco-Customer-Churn.csv
│   ├── X_processed.csv
│   └── y_processed.csv
│
├── notebooks/
│   └── 01_eda.ipynb
│
├── src/
├── models/
├── visualizations/
│
├── README.md
└── PROJECT_PROGRESS.md
```

Additional files and notebooks may be added as the project develops.

## 8. EXPECTED FINAL DELIVERABLES

- Cleaned and processed dataset
- Exploratory Data Analysis notebook
- Feature engineering and preprocessing workflow
- Trained Machine Learning models
- Model evaluation and comparison
- Final selected model
- Customer churn prediction system
- Project visualizations
- GitHub documentation

## 9. LEARNING OUTCOMES

By completing this project, the following concepts and skills will be practiced:

- Data cleaning and preprocessing
- Exploratory Data Analysis
- Feature engineering
- Categorical encoding
- Classification algorithms
- Training and testing datasets
- Model evaluation
- Class imbalance handling
- Model improvement
- Python programming with Pandas and Scikit-learn
- GitHub project management

## 10. PROJECT STATUS

This project is being developed as a 10-day hands-on Machine Learning project.

Completed:
- Day 1: Project Setup and Dataset Collection
- Day 2: Exploratory Data Analysis
- Day 3: Data Cleaning and Preprocessing
- Day 4: Feature Engineering and Data Preparation
- Day 5: Logistic Regression Model

Current Model:
- Algorithm: Logistic Regression
- Initial Test Accuracy: 80.38%

The model will be further evaluated and compared with other classification algorithms.
