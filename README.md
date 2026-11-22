# 📉 Telecom Customer Churn Analysis

Cleaning a messy telecom dataset with **pandas** and visualising it with a **stack plot** and a **donut pie chart** in **matplotlib**.

## Dataset
`telecom_churn.csv` (2,540 rows, synthetic) with customer details, contract type, internet service, charges, support calls, churn status and churn reason.

## What I Did
- **Cleaning:** removed duplicates, fixed `gender` text, replaced invalid charges (-1), filled missing values (`groupby` + `transform`)
- **Features:** `signup_month`, `age_group` (`pd.cut`), `churn_flag`
- **Charts:** stack plot of new customers per month by contract type, and a donut pie chart of churn reasons, combined in one dashboard

## Dashboard
![Churn Dashboard](churn_dashboard.png)

## Key Insights
- **Month-to-month + Fiber** customers have the highest churn rate
- Churned and retained customers pay almost the same, so price is not the main reason
- **36-50** has the most churners; **26-35** has the highest churn rate

## Run
```bash
pip install pandas numpy matplotlib
jupyter notebook churn_analysis.ipynb
```

## Tech
Python · pandas · NumPy · matplotlib

## Author
Shantanu· shantanuthakur2010-bit
