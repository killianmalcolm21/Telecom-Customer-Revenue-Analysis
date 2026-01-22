# Telecom Customer Revenue Analysis

## Overview
This project analyzes customer usage behavior and revenue generation for a mobile telecom provider offering two subscription plans: Surf and Ultimate. The goal is to determine which plan is more profitable and to understand how customer behavior, pricing structure, and geography influence revenue.

The analysis combines data cleaning, feature engineering, revenue modeling, descriptive statistics, visualization, and hypothesis testing to produce business-ready insights.

---

## Dataset
The dataset includes:
- Call records (duration and timestamps)
- Message records
- Internet usage sessions
- Customer subscription details
- Pricing and plan allowances
- Customer location and churn information

All usage data was aggregated to a **monthly, per-user level** to align with telecom billing practices.

---

## Key Steps
1. **Data Cleaning & Preparation**
   - Standardized data types and handled missing values
   - Converted raw usage into billable units (minutes, GB)
   - Verified data quality across all datasets

2. **Feature Engineering**
   - Aggregated calls, messages, and internet usage per user per month
   - Applied plan limits and overage pricing
   - Calculated total monthly revenue per user

3. **Exploratory Data Analysis**
   - Compared usage behavior across plans
   - Visualized distributions for calls, messages, internet usage, and revenue
   - Identified variability and overage patterns

4. **Statistical Analysis**
   - Tested whether average revenue differs by plan
   - Tested whether average revenue differs between NY–NJ and other regions
   - Used Welch’s t-test with a significance level of α = 0.05

---

## Key Findings
- Ultimate users consume more services on average but generate more stable revenue due to higher included allowances.
- Surf users show greater variability in usage, leading to more frequent overage charges and higher marginal revenue.
- The difference in average monthly revenue between plans is **statistically significant**.
- Revenue in the NY–NJ region differs significantly from other regions, indicating potential geographic effects.

---

## Business Implications
- Usage variability is a stronger revenue driver than average consumption.
- Lower-priced plans with overage charges can outperform premium plans in profitability.
- Geographic segmentation may be useful for pricing and marketing strategy.

---

## Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- SciPy

---

## Author
**Lawrence Malcolm Killian**  
Data Analyst / Data Scientist  
