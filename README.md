# Customer Churn & Retention Analysis

## Project Overview

This project analyzes a telecommunications customer dataset to investigate customer churn and identify characteristics associated with customer retention.

The goal is to use Python and Pandas to clean, explore, and analyze customer data, then communicate findings that could inform business retention strategies.

**Project Status:** In Progress — Data Exploration and Cleaning Completed

## Tools & Technologies

- Python
- Pandas
- Jupyter Notebook
- Matplotlib and Seaborn (planned)
- Git and GitHub

## Dataset

**Source:** Telco Customer Churn — IBM Sample Dataset, distributed on Kaggle

The dataset contains 7,043 customer records and 21 columns, including customer demographics, contract information, subscribed services, monthly charges, total charges, and churn status.

## Business Questions

1. What percentage of customers have churned?
2. Which contract types have the highest churn rates?
3. How does customer tenure relate to churn?
4. Is there a relationship between monthly charges and churn?
5. Which customer segments could benefit from targeted retention programs?

## Project Progress

### 1. Data Exploration — Completed

- Imported and inspected the dataset using Pandas.
- Examined column names, data types, and descriptive statistics.
- Identified 7,043 customer records and 21 columns.
- Calculated the overall customer churn rate.

**Initial finding:** 1,869 customers (26.54%) churned, while 5,174 customers (73.46%) did not.

### 2. Data Cleaning — Completed

- Identified 11 blank values in `TotalCharges`.
- Converted `TotalCharges` from a string to a numeric data type.
- Found that all 11 affected customers had a tenure of zero months.
- Replaced missing `TotalCharges` values with zero, based on an assumption that these customers had not yet accumulated charges.
- Checked for duplicate customer records and customer IDs; none were identified.
- Converted `SeniorCitizen` from numeric codes into readable Yes/No labels.

### 3. Exploratory Data Analysis — In Progress

Upcoming analysis will investigate churn rates by contract type, tenure, monthly charges, and internet service type.

### 4. Data Visualization — Planned

Create visualizations that communicate key relationships and findings.

### 5. Business Recommendations — Planned

Summarize important findings and suggest potential customer retention strategies.

## How to Run

1. Download the Telco Customer Churn dataset from Kaggle.
2. Place `WA_Fn-UseC_-Telco-Customer-Churn.csv` inside the `data/` folder.
3. Install Python, Pandas, and Jupyter Notebook.
4. Open `churn_analysis.ipynb` from the project root directory.
5. Run the notebook cells in order.

## Limitations

This is a sample customer dataset rather than current production data. Because it contains customer-level observations rather than a complete longitudinal customer history, relationships should not automatically be interpreted as causal explanations for churn.

## Next Steps

- Analyze customer churn by contract type.
- Investigate relationships between churn, tenure, and monthly charges.
- Create visualizations.
- Develop business recommendations.
- Present final findings and project conclusions.
