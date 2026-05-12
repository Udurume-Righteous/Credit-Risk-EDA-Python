# Credit Risk EDA Using Python

## Project Overview

This project presents an end-to-end **Exploratory Data Analysis (EDA)** of borrower credit and loan repayment behavior using Python. The goal of the analysis is to understand the factors influencing loan repayment outcomes and identify patterns associated with loan defaults (charged-off loans).

The project demonstrates a complete data analysis workflow, including:

- Data cleaning and preprocessing
- Missing value handling
- Duplicate detection and removal
- Feature engineering
- Univariate and bivariate analysis
- Correlation analysis
- Business insight extraction


---

## Dataset Information

The dataset contains **100,000 loan records** with borrower financial, credit, and loan-related information.

### Features include:

- Loan Status
- Credit Score
- Annual Income
- Loan Amount
- Monthly Debt
- Years in Current Job
- Home Ownership
- Loan Purpose
- Credit History
- Delinquency History
- Credit Problems
- Bankruptcies
- Tax Liens

---

## Project Objectives

The analysis aims to answer the following business questions:

- What factors are associated with successful loan repayment?
- Are long-term loans riskier than short-term loans?
- Does credit score influence repayment outcomes?
- Do borrowers with higher debt burdens default more frequently?
- Which loan purposes exhibit higher repayment risk?
- Does housing ownership influence loan performance?

---

## Data Cleaning & Preprocessing

The following cleaning steps were performed:

### Data Quality Improvements

- Removed **10,215 duplicate rows**
- Corrected wrongly scaled **credit scores**
- Replaced placeholder values (`99999999`) in loan amount records
- Standardized categorical values in **Home Ownership**
- Converted **Years in Current Job** into numerical format
- Preserved informative missing values in:
  - `Months since last delinquent`

### Missing Value Handling

- Median imputation for skewed numerical variables
- Mode imputation for categorical variables
- Delinquency history values intentionally retained to preserve business meaning

---

## Exploratory Data Analysis

### Univariate Analysis
Analysis of:

- Loan Status
- Loan Term
- Home Ownership
- Loan Purpose
- Credit Score
- Income Distribution
- Monthly Debt
- Loan Amount

### Bivariate Analysis
Comparison of borrower characteristics against:

**Loan Status**

Including:

- Credit Score vs Loan Status
- Annual Income vs Loan Status
- Debt-to-Income Ratio vs Loan Status
- Loan Term vs Loan Status
- Home Ownership vs Loan Status
- Loan Purpose vs Loan Status

---

## Feature Engineering

A new financial metric was created:

### Debt-to-Income Ratio (DTI)

```python
Debt_to_Income_Ratio = (Monthly Debt × 12) / Annual Income
```

This feature was used to investigate financial burden and repayment performance.

---

## Key Findings

### 1. Most borrowers successfully repay loans
Approximately **75% of loans were fully paid**, while roughly **25% resulted in charge-offs**.

### 2. Long-term loans are riskier
Long-term loans exhibited substantially **higher charge-off rates** than short-term loans.

### 3. Debt consolidation dominates borrowing behavior
Nearly **79% of borrowers** requested loans for **debt consolidation**, suggesting financial restructuring as the primary borrowing motive.

### 4. Credit score influences repayment
Borrowers with **higher credit scores** generally demonstrated stronger repayment performance.

### 5. Renters exhibited slightly higher repayment risk
Borrowers under **Rent** showed slightly elevated charge-off rates compared to homeowners and mortgage holders.

### 6. Debt burden matters
Borrowers with **higher Debt-to-Income Ratios (DTI)** were more likely to experience repayment difficulties.

### 7. Job duration showed limited predictive impact
Employment duration did not exhibit a strong relationship with repayment outcomes.

### 8. Financial distress indicators are strongly related
Strong correlation was observed between:

- Credit Problems and Bankruptcies
- Credit Problems and Tax Liens

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- Jupyter Notebook

---

## Repository Structure

```text
Credit-Risk-EDA-Python/
│── Credit_EDA.ipynb
│── cleaned_credit_data.csv
│── credit.csv
│── README.md
```

---

## Conclusion

This project demonstrates a complete **end-to-end exploratory data analysis workflow** for understanding borrower credit behavior and repayment risk.

The findings suggest that loan repayment outcomes are influenced by multiple interacting financial factors, particularly **loan duration, debt burden, creditworthiness, and financial distress indicators**.

This analysis highlights practical skills in **data cleaning, visualization, feature engineering, statistical reasoning, and business insight extraction using Python**.

---

## Author

**Righteous Udurume**  
Data Analyst | Data Scientist  

Passionate about transforming raw data into actionable insights through **data analysis, machine learning, and data-driven problem solving**.

**Skills:**  
Python • SQL • Data Analysis • Data Visualization • Machine Learning • Exploratory Data Analysis (EDA) • Power BI • Data Cleaning • Statistical Analysis
