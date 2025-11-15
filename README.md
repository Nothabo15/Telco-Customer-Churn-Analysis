> # Telco-Customer-Churn-Analysis 2024
> Data analysis and visualization of customer churn for a telecom company

> ## Client Overview

> The Telco company is a large telecommunications provider offering internet, phone, and streaming services across multiple regions. Like most subscription-based businesses, profitability depends on long-term customer retention, predictable recurring revenue (MRR), and the ability to reduce churn across high-value segments.

> The Telco Churn Dashboard 2024 consolidates customer behavior, contract types, service usage, revenue contribution, and churn risk into a single analytics view. The goal is to provide a clear understanding of why customers leave, which customer groups are at highest risk, and what strategies can improve retention and lifetime value (CLV).

> ## Business Objectives

> 1. Identify customer segments with the highest churn risk.

> 2. Understand how contract type, payment method, internet service, and tech support influence churn.

> 3. Quantify revenue impact by measuring MRR at risk and customer lifetime value (CLV).

> 4. Support data-driven retention strategies that reduce voluntary churn.

> 5. Enable the business to forecast churn trends and prioritize high-value customer retention.

> ## Key Metrics

> - Churn Rate: 26.58% — significantly above the industry benchmark of ~20%.

> - MRR at Risk: ~$139K monthly, representing 27% of total monthly revenue at stake.

> - Average Customer Lifetime Value: $2,100 — higher for retained customers (~$2,555).

> - Contract Impact: Month-to-month customers show the highest churn rate.

> - Service Impact: Fiber Optic users churn at the highest rate compared to DSL or No Internet plans.

> ## Customer & Revenue Insights
![Telco Customer Churn Dashboard](https://github.com/Nothabo15/Telco-Customer-Churn-Analysis/blob/main/Telco%20Churn%20Dashboard.png?raw=true/TelcoChurnDashboard.png)

> This dashboard provides a comprehensive analysis of customer churn, revenue at risk, and the key drivers contributing to customer attrition in a telecommunications company.
> The key KPIs are:
> - Churn Rate: 26.58% which is more than a quarter of customers leaving the service.
> - Total Customers are 7032
> - MRR at Risk at 30.53% shows that monthly revenue is threatened by churn.

> ## Churn by Contract Type

> - Month-to-Month customers generate the highest churn rate at 42.71%.
> - One-Year & Two-Year contracts show significantly lower churn confirming that commitment length directly impacts retention.
> - Recommendation: Incentivize upgrades to long-term contracts.

> ## Churn by Payment Method

> - Electronic Check customers churn at the highest rate (45.29%).
> - Customers using credit cards and bank transfers show better retention.
> - Recommendation: We can promote automatic billing setups to reduce churn.

> ## Internet Service Impact

> - Fiber Optic users churn most at 41.89% potentially due to price sensitivity or service expectations.
> - DSL and non-internet customers show lower churn.
> - Recommendation: We can offer loyalty discounts or improved support for fiber optic customers.

> ## Tenure-Based Churn Behavior

> - Customers in their first 12 months are most likely to churn, as shown the short term customers churned at 47.68%. 
> - As tenure increases, churn drops sharply.
> - Recommendation: Strengthen onboarding and early customer engagement programs.

> ## Key Findings

> - Month-to-month customers and fiber optic users are high-risk churn groups.
> - First-year customers are the most vulnerable segment (critical retention window).
> - Electronic check users churn due to billing inconvenience.
> - High-fee customers churn more, highlighting pricing pain points.
> - Tech Support significantly reduces churn across all demographics.
> - ~$139K in monthly revenue is at risk, driven primarily by churned high-value users.

> These insights highlight that Telco’s biggest opportunities lie in improving customer onboarding, promoting long-term contracts, optimizing pricing tiers, and strengthening service support.

> ## Key Takeaways
> **1. Strengthen Early Retention Programs**

> The first 12 months represent the highest churn risk, proactive engagement can dramatically improve retention.

> **2. Drive Long-Term Contract Adoption**

> Long-term contract customers show far lower churn and generate stable recurring revenue.

> **3. Improve Billing Convenience**

> Shifting electronic-check customers to auto-pay channels can reduce churn significantly.

> **4. Support High-Value Segments**

> Fiber optic users and high-paying customers need targeted retention strategies (discounts, VIP support).

> **5. Bundle Value-Added Services**

> Tech Support and Security add-ons increase stickiness and reduce churn.

> ## Data Cleaning & Preparation

> I sourced this dataset from Kaggle and prepared it in SQLite before visualizing it in Tableau. In this process I ensured accuracy, consistency, and analytical readiness.

> **1. Data Import & Initial Review**

> I Imported the Telco Customer Churn dataset into SQLite for structured analysis and for quick assessment.

> **2. Data Quality Checks**
> -	Checked for duplicate customer records none were found.
> -	Identified blanks in TotalCharges and whitespace in categorical fields trimmed text & filtered invalid rows.
> -	Standardized Yes/No fields and fixed inconsistent text formatting	Applied TRIM + normalization
> - Converted TotalCharges (string → numeric)	CAST applied and validated
> - Removed records with tenure = 0 or TotalCharges = 0 to ensure valid customer tenure.
> - Created a cleaned table: telco_churn_cleaned.

> **3. Calculated Fields Added**

> To support advanced analytics:

> Average Customer Lifetime Value (CLV):
> CLV = MonthlyCharges * Tenure

> MRR at Risk:
> Sum of MonthlyCharges for churned customers.

> Tenure Groups: 0–1 yr, 1–2 yrs, …, 5+ yrs

> Price Categories: Low, Medium, High, Very High

> Churn Flags for segmentation

> ## Tools & Technologies
> - SQLite for Data preparation & cleaning
> - Tableau Public	Dashboard creation & visual analytics
> - GitHub	Project documentation & portfolio

> ## Executive Summary

> The Telco Churn Analysis reveals a 26.58% churn rate, driven primarily by short-term contracts, early-tenure customers, fiber optic services, and billing friction. High-value customers are disproportionately represented in churn totals, putting 27% of monthly recurring revenue at risk.

> Strategic focus should emphasize:

> - Early-tenure retention

> - Contract upgrades

> - Billing simplification

> - Improved fiber optic support

> - Targeted outreach for high-CLV customers

> This analysis demonstrates how churn analytics can transform raw telecom data into actionable retention strategies that protect revenue and strengthen customer loyalty.

> ## Business Relevance

> These insights help the Telco business:

> - Predict churn across service segments

> - Prioritize high-risk customers for retention programs

> - Improve pricing and contract strategies

> - Reduce revenue leakage

> - Strengthen long-term customer relationships

> ## Explore the Interactive Dashboard

>  Link to Tableau Public (https://public.tableau.com/app/profile/nothabo.moyo)

> ## Author

> **Nothabo Michelle Moyo**
> Data Analyst | SQL • Excel • Tableau
> nothabomoyo07@gmail.com

> ## 🔗 LinkedIn: https://www.linkedin.com/in/nothabo-michelle-moyo-a38840378/
