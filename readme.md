# 💳 Credit Risk Analytics Dashboard

## 📌 Overview

This project aims to provide a data-driven solution to assess credit risk and analyze banking metrics using **Power BI**. By integrating various client and banking-related data, I have built a suite of dashboards to help financial institutions **minimize loan default risks** and **monitor key banking KPIs**.

---

## 🧠 Problem Statement

Develop a foundational understanding of **risk analytics in banking** and explore how data can drive informed decisions in lending — approving loans only when the applicant is likely to repay.

---

## 📊 Dataset

The dataset consists of multiple **interconnected tables** representing banking relationships and client profiles:

- `Banking Relationship`
- `Clients`
- `Gender`
- `Investment Advisor`
- `Period`

The tables are linked using **primary** and **foreign keys**.

---

## 🛠️ Key Features & Steps

### 🔧 Data Cleaning & Feature Engineering

- Created `Engagement Timeframe` and `Engagement Days` columns to track customer lifetime.
- Binned income into `Income Band` categories:
  - Low (< ₹100,000)
  - Mid (< ₹300,000)
  - High (> ₹300,000)
- Derived `Processing Fees` based on the fee structure (e.g., 0.05 for high fee).

---

### 🧮 DAX Measures Used

- **SUM**, **SUMX**, **DISTINCTCOUNT**, **SWITCH**, **DATEDIFF**
- Example KPIs:
  - `Total Clients = DISTINCTCOUNT(Client ID)`
  - `Total Loan = Bank Loan + Business Lending + Credit Card Balance`
  - `Total Fees = SUMX(Clients, Total Loan * Processing Fees)`
  - And many more

---

### 📈 Dashboards & Visualizations

- **Home Dashboard**
- **Loan Analysis**
- **Deposit Analysis**

These dashboards offer clear insight into the financial health and engagement of clients.

---

## 🧩 Tools & Technologies

- Python (Exploratory Data Analysis)
- Power BI (Data Modeling & Visualization)
- DAX (Data Analysis Expressions)
- Relational Data Modeling (via Power BI’s data view)

---

## ✅ Key Insights

- Processing fees scale with the total loan amount.
- Private banks have a larger customer base.
- Nationality trends indicate specific countries with higher loan demands.
- Income levels and client engagement days are strong indicators of lending risk.

---

## 🚀 Future Scope

- Automate alerts for high-risk clients based on dashboard thresholds.
- Integrate ML models to predict default probability.
- Use segmentation to offer tailored banking services.

---

Feel free to explore the repo and reach out with feedback or collaboration ideas!
