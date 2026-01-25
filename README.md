# Telecom Customer Revenue Analysis & Plan Profitability

## Project Overview
This project analyzes customer usage behavior and revenue generation for a telecom company offering two mobile plans: **Surf** and **Ultimate**. The goal is to determine which plan is more profitable and understand how customer behavior (calls, messages, and internet usage) impacts revenue under real billing rules.

The analysis combines data cleaning, aggregation, exploratory analysis, revenue modeling, and statistical hypothesis testing to support a data-driven business recommendation.

---

## Business Objective
- Compare **monthly revenue** between the Surf and Ultimate plans  
- Understand **customer usage patterns** by plan  
- Determine which plan is **more profitable and sustainable**  
- Validate conclusions using **statistical hypothesis testing**

---

## Data Description
The dataset includes usage data for 500 customers across 2018:
- **Calls:** duration and timestamps  
- **Messages:** message counts and timestamps  
- **Internet:** data usage in MB  
- **Plans:** pricing and included allowances  
- **Users:** plan type, region, churn information  

All data was aggregated to a **per-user, per-month** level to support revenue analysis.

---

## Methodology
1. **Data Preparation**
   - Cleaned and standardized data types
   - Handled missing values appropriately (e.g., churn dates)
   - Created monthly aggregates for calls, messages, and internet usage

2. **Feature Engineering**
   - Rounded call durations per billing rules
   - Converted MB → GB for internet usage
   - Merged usage data with plan pricing

3. **Revenue Calculation**
   - Computed monthly revenue per user based on plan limits and overage fees
   - Combined call, message, and internet charges with fixed monthly fees

4. **Exploratory & Behavioral Analysis**
   - Compared usage distributions by plan
   - Visualized revenue, message, and internet usage patterns
   - Identified differences in customer behavior across plans

5. **Statistical Hypothesis Testing**
   - Tested whether average monthly revenue differs between plans
   - Applied a two-sample t-test with a 5% significance level

---

## Key Findings
- **Surf plan users** tend to exceed included limits more frequently, generating higher variability in revenue.
- **Ultimate plan users** show more stable usage patterns with fewer overages.
- Despite higher base pricing, the **Ultimate plan generates higher average monthly revenue**.
- Statistical testing confirms that the difference in mean revenue between plans is **statistically significant**.

---

## Hypothesis Testing Result
- **Null Hypothesis (H₀):** Average monthly revenue is the same for both plans  
- **Alternative Hypothesis (H₁):** Average monthly revenue differs between plans  

The null hypothesis was **rejected**, indicating a significant difference in revenue between Surf and Ultimate users.

---

## Final Business Recommendation
Based on revenue modeling, customer behavior analysis, and statistical testing, the **Ultimate plan is more profitable and financially stable**. It produces higher average monthly revenue with lower variability, making it the stronger plan from a business perspective.

---

## Tools & Technologies
- Python  
- pandas, NumPy  
- matplotlib  
- SciPy (hypothesis testing)

---

## How to Run
1. Clone the repository  
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib scipy
## Author: Lawrence Malcolm Killian
