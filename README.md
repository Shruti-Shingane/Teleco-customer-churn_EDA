# Teleco-customer-churn_EDA
Readme · MD
Telco Customer Churn – Exploratory Data Analysis
Overview

This project explores the Telco Customer Churn dataset to understand the key factors driving customer attrition at a telecom company. Through data cleaning, univariate, numerical, and bivariate analysis, the project identifies which customer attributes are most strongly associated with churn — and which ones aren't.

Dataset
Source: Telco Customer Churn dataset (CustomerChurn.csv)
Size: 7,043 customers, 21 features
Target variable: Churn (Yes/No)
Features include: demographics (gender, senior citizen, partner, dependents), account info (tenure, contract type, payment method, charges), and services subscribed (internet, phone, security, streaming, etc.)
Objective

To perform exploratory data analysis and answer:

What is the overall churn rate?
Which customer segments are most likely to churn?
Which factors have little to no impact on churn?
What patterns emerge when combining multiple variables (e.g., charges, tenure, contract type)?
Process

1. Data Cleaning

i) Converted TotalCharges from object to numeric type

ii) Dropped 11 rows with missing TotalCharges (0.15% of data — negligible impact)

iii) Binned continuous tenure into groups (1–10, 11–20, ... 71–80) for clearer visualization

iv) Dropped customerID and raw tenure after creating tenure groups

2. Univariate Analysis

i) Examined churn distribution and missing values

ii) Visualized each categorical feature against churn using count plots

3. Numerical Analysis

i) Explored MonthlyCharges and TotalCharges distributions by churn status (KDE plots)

ii) Computed correlation of numeric and one-hot encoded features with churn

iii) Visualized correlations with a heatmap and bar chart

4. Bivariate Analysis

Broke down churn by gender within key segments (partner status, payment method, contract type) to uncover deeper patterns
Key Insights

Higher churn is associated with:

i) Month-to-month contracts (no lock-in period)

ii) Low tenure — new customers churn far more than long-tenured ones

iii) No online security or tech support subscribed

iv) Fiber optic internet service

v) Senior citizens

vi) Electronic check as payment method

vii) High Monthly Charges paired with low Total Charges — a signature of new customers on expensive plans who leave before their spend accumulates

Lower / no impact on churn:

i) Long-term (especially 2-year) contracts

ii) 5+ years of tenure

iii) No internet service subscribed

iv) Gender, phone service, and multiple lines — minimal to no relationship with churn

Bivariate findings:

i) Among customers without a partner, females churn slightly more; among those with a partner, males churn slightly more 

ii)Among electronic check users, males churn more than females

Tech Stack :-

Python

Pandas, NumPy (data manipulation)

Matplotlib, Seaborn (visualization)

Jupyter Notebook




Shruti Shingane
