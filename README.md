Retail Mortgage Early-Warning & Portfolio Risk Engine

📌 Executive Summary

This project simulates a retail banking environment to identify early-warning indicators for Non-Performing Assets (NPAs) within a mortgage loan portfolio. By architecting a relational database of 10,000 synthetic loan accounts, I developed an SQL-based analytical pipeline that identified an 8.3% default vulnerability concentrated within specific geographic and employment segments, allowing for targeted credit policy adjustments.

🏦 Business Problem

Retail banks are aggressively expanding home loan books into Tier-2 and Tier-3 markets. However, underwriting standards applied to Tier-1 salaried employees do not always translate to self-employed individuals in emerging markets, leading to invisible risk concentration and EMI bounce rate spikes.

🛠️ Methodology & Tech Stack

Data Engineering (Python/Pandas): Engineered a highly realistic, relational dataset of 10,000 retail mortgage accounts across 3 tables (applicants, loan_terms, repayment_history). Embedded statistical correlations between CIBIL scores, Loan-to-Value (LTV) ratios, and subsequent EMI bounce probabilities.

Data Architecture (SQL): Designed an in-memory SQL database. Utilized Common Table Expressions (CTEs), multi-table joins, and conditional aggregation to isolate accounts with 3+ rolling EMI bounces.

Data Visualization (Matplotlib/Seaborn): Developed executive-ready visual summaries highlighting risk bifurcation across segments.

📊 Key Findings

Risk Concentration: The Self-Employed (Tier 3) segment represents the highest risk exposure at an 8.30% NPA probability.

Safety Buffer: The Salaried (Tier 2) segment is the safest cohort, with a near-zero 0.54% NPA probability, suggesting room to aggressively expand marketing in this sector.

The "Hidden" Threat: Despite a large volume of loans (1,709 accounts), the Self-Employed (Tier 2) segment carries a dangerously high 7.96% NPA risk, indicating current underwriting models for this specific group are failing.

💡 Credit Policy Recommendations

Tighten LTV Limits: Cap maximum Loan-to-Value ratios at 55-60% based on the type of property mortgaged for all self-employed applicants in Tier 3 markets.

Pricing Adjustments: Increase the risk premium on interest rates by 50 basis points for Self-Employed applicants in Tier 2/Tier 3 cities who possess a CIBIL score below 710.

Marketing Shift: Reallocate customer acquisition budgets toward Tier-2 Salaried professionals to balance portfolio risk.

Note: This project relies on synthetically generated data to respect data privacy laws while demonstrating advanced analytics capabilities applicable to real-world financial institutions.
