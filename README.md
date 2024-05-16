# Lending Data Analysis and Logistic Regression Model
This project involves analyzing a lending dataset and building a logistic regression model to predict loan statuses. The model distinguishes between healthy loans (0) and high-risk loans (1).

### Table of Contents
- Overview
- Data
- Project Steps
- 1. Data Loading
- 2. Data Preprocessing
- 3. Train-Test Split
- 4. Model Training
- 5. Model Evaluation
- Results
- Usage

# Overview
The objective of this project is to create a logistic regression model to predict whether a loan is healthy or high-risk based on various features. The model's performance is evaluated using metrics such as accuracy, precision, recall, and the F1-score.

# Data
The dataset lending_data.csv is used, which contains the following columns:

- loan_size: The size of the loan
- interest_rate: The interest rate of the loan
- borrower_income: The income of the borrower
- debt_to_income: The debt-to-income ratio of the borrower
- num_of_accounts: The number of accounts the borrower has
- derogatory_marks: The number of derogatory marks on the borrower's credit report
- total_debt: The total debt of the borrower
- loan_status: The status of the loan (0 = healthy, 1 = high-risk)

# Project Steps
1. ### Data Loading
The data is loaded from the Resources folder into a Pandas DataFrame.
import pandas as pd
from pathlib import Path

Load the data
df = pd.read_csv(Path("Resources/lending_data.csv"))

2. ### Data Preprocessing
The labels (y) are separated from the features (X).
