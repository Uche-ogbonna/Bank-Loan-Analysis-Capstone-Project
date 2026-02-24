# Bank-Loan-Analysis-Capstone-Project
This capstone project focuses on analyzing bank loan data to uncover patterns in loan performance, borrower behavior, and credit risk. The primary goal of this project is to transform raw financial loan data into actionable business insights using data modeling, transformation, and interactive dashboard development in Power BI.
# Loan Analysis Capstone Project

## 📄 Project Overview

This project analyzes a dataset of loan applications to uncover key insights about lending patterns, borrower behavior, and portfolio risk. The analysis focuses on:

- Loan defaults and repayment patterns
- Borrower debt-to-income (DTI) and income verification
- Loan trends over time
- Geographic distribution of loans
- Loan amounts and installment patterns by loan grade, term, and purpose

The project uses **Power BI** for visualization and **Excel** for cleaned data preparation.

---

## 🗂️ Repository StructureLoan-Analysis-Project/
│
├─ data/
│ ├─ loan_data_raw.xlsx # Original dataset
│ └─ loan_data_cleaned.xlsx # Cleaned and preprocessed data
│
├─ reports/
│ ├─ Loan_Analysis_Report.pbix # Full Power BI report
│ └─ Loan_Analysis_Dashboard.pbix # Dashboard-only version
│
└─ README.md # This file
---

## 🧹 Data Cleaning

- Removed missing or inconsistent values in key columns (loan amount, term, DTI, emp_length)
- Standardized employment length into categories: `<1 year`, `1-5 years`, `6-10 years`, `10+ years`
- Ensured numeric columns are formatted correctly for analysis
- Created a **duplicate table** in Power BI for cleaned data, independent of the original table
- Exported the cleaned table to Excel (`loan_data_cleaned.xlsx`) for reproducibility

---

## 📊 Key Analysis & Visuals

### 1. **Loan Trends Over Time**
- Line chart showing number of loans issued by month/year
- Highlights periods of increased or decreased lending activity

### 2. **Average Loan Amount by Grade**
- Clustered column chart
- Charged-off loans tend to have higher average loan amounts than fully paid loans:
  - Charged Off → $12,288.06  
  - Fully Paid → $10,930.42

### 3. **Default Rates**
- Calculated as:Default Rate = (Number of Charged-Off Loans) / (Total Loans) × 100%- Can be segmented by:
  - Loan grade
  - Verification status
  - Purpose
  - State

### 4. **Average DTI and Installment by Loan Status**
- Charged-off loans have higher average DTI and installment amounts, indicating higher financial stress

### 5. **Loan Volume by State**
- Map / Heat map visual showing concentration of loans across states
- Identifies high-demand regions

### 6. **Total Repayment by Loan Purpose**
- Sum of `total_pymnt` for each purpose category
- Highest repayment category typically indicates the most significant cash inflow segment

### 7. **Filters & Slicers**
- Interactive slicers for **Term**, **Grade**, and **Purpose**
- All visuals update dynamically based on slicer selections

---

## 💡 Insights

- **Higher loan amounts** are associated with higher default rates
- **Non-verified applicants** tend to default more than verified ones
- **Shorter-term loans** (36 months) have higher installments but may carry less default risk
- **Debt consolidation** is often the purpose with the highest number of loans and total repayment
- States like **California** (example) have the largest loan volumes, reflecting geographic concentration

---

## 🛠️ How to Use This Repository

1. Open `loan_data_cleaned.xlsx` to explore the cleaned dataset in Excel
2. Open `Loan_Analysis_Report.pbix` in Power BI Desktop to view full report
3. Use slicers to filter by **Term**, **Grade**, and **Purpose** for segmented analysis
4. Export visuals or data for reporting or presentation purposes

---

## 📁 Notes

- **Duplicate tables** were used in Power BI to preserve clean data independently of the raw dataset
- Sensitive personal information has been anonymized or removed
- All analysis is based on the cleaned dataset for reproducibility

---

## 📌 References

- Power BI Desktop: [https://powerbi.microsoft.com/](https://powerbi.microsoft.com/)
- Excel 365 or newer for CSV/Excel exports


