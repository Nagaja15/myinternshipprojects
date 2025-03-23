# myinternshipprojects
# Bank Churn Prediction

This project aims to predict customer churn for a bank using various machine learning models. The dataset includes customer details such as credit score, age, tenure, balance, and more, with the goal of identifying whether a customer will exit (churn) or stay.

## Project Overview

The Jupyter Notebook `Churn_Prediction.ipynb` walks through the entire process:
- **Data Preprocessing**: Handling duplicate columns, encoding categorical variables (`Geography`, `Gender`), and scaling numeric features.
- **Model Evaluation**: Comparing six classifiers (Logistic Regression, Decision Tree, Random Forest, KNN, Gaussian Naive Bayes, XGBoost) using 5-fold cross-validation.
- **Metrics**: Accuracy, precision, and recall are calculated for each model to assess performance.

The best-performing model is Random Forest, achieving an average accuracy of ~86%.

## Files

- **`Churn_Prediction.ipynb`**: Main Jupyter Notebook containing the code, outputs, and explanations.
- **`Churn_Modelling.csv`** (optional): The dataset used for training and evaluation. If not included, download it from [Kaggle: Bank Customer Churn Prediction](https://www.kaggle.com/datasets/shubhammeshram579/bank-customer-churn-prediction) or replace with your own file.
- **`requirements.txt`**: List of Python dependencies required to run the notebook.

## Dataset

The dataset contains 10,000 rows with the following original columns (before preprocessing):
- `RowNumber`, `CustomerId`, `Surname` (dropped as irrelevant)
- `CreditScore`, `Geography`, `Gender`, `Age`, `Tenure`, `Balance`, `NumOfProducts`, `HasCrCard`, `IsActiveMember`, `EstimatedSalary`, `Exited` (target)

After preprocessing:
- `Geography` → `Geography_Germany`, `Geography_Spain` (France as baseline)
- `Gender` → `Gender_Male` (Female as baseline)
- Numeric features scaled for better model performance.

## Requirements

To run the notebook, install the following Python packages:
pandas,numpy,seaborn......

Install them using:
```bash
pip install -r requirements.txt
How to Run
Clone the Repository:
bash
Collapse
Copy
git clone https://github.com/Nagaja15/Bank-Churn-Prediction.git
cd Bank-Churn-Prediction
