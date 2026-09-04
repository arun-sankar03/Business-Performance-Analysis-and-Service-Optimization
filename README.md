# Business Performance Analysis and Service Optimization: A Primary Data Study of a Professional Laundry Business

BDM Capstone Project (IIT Madras, BS Data Science and Applications) analyzing 2,607 primary customer order records from RDS Associates ("Rinz n Dry"), a dry-cleaning and laundry business in Thrissur, Kerala, to address revenue imbalance, operational efficiency, and customer retention.

## Overview

This project uses primary data collected directly from a B2C laundry business (operating since 2022) to analyze three problem statements:
1. **Revenue and Service Demand Imbalance** — which services drive revenue vs. volume
2. **Operational Efficiency and Turnaround Time (TAT)** — service policy, peak demand, complaint trends
3. **Customer Retention and Behavioural Patterns** — loyalty, repeat visits, cohort retention

Data spans 10 March 2026 – 10 July 2026 (106 working days, Monday–Saturday), with 16 columns covering order timing, customer type, service, billing, delivery, TAT, and complaint status.


## Workflow

1. **Data Collection** — primary data via interviews (operational data) and exported digital records (2,607 customer order records), with organizational permission letter.
2. **Data Cleaning & Validation** — duplicate detection, missing value checks, date/range consistency, outlier screening, aggregate cross-verification against manual registers.
3. **Descriptive Statistics** — service-wise order/revenue distribution, numerical variable summaries, monthly revenue normalization.
4. **Hypothesis Testing & Correlation** — t-tests, chi-square, ANOVA, Pearson correlation with significance testing to validate patterns (not assume causation).
5. **Time Series Analysis** — weekly revenue stability trend (16 complete weeks).
6. **Advanced Segmentation (Final phase)** — ABC/Pareto revenue classification, revenue-per-garment density analysis, hour×weekday demand heat-map, monthly complaint trend, customer order-frequency tiers, acquisition-cohort retention analysis, complaint-resolution vs. repeat-behaviour analysis.

## Key Findings

- **Wash & Iron** dominates: 47.8% of orders, 62.9% of revenue (Rs. 8,24,685) — the single Class-A service.
- **TAT is policy-driven, not size-driven**: Normal orders = 4 days, Express = 1 day (zero variance); correlation with order size is weak (r = -0.165, p < 0.001).
- **Express service** is an underused premium lever — 56.5% higher average bill, only 11.4% of order volume.
- **Regular customers** (46.4% of base) drive 78.4% of orders and 79% of revenue — through frequency, not larger baskets (t-test p = 0.166).
- **Peak demand**: Wednesday 9–10 AM (87 orders) and Monday 10–11 AM (82 orders) are the sharpest peaks.
- **Complaint rate**: 14.4% overall, 90.7% resolved; customers with a resolved first-order complaint return at a *higher* rate (89.9%) than those without complaints (61.2%) — complaint resolution acts as a retention mechanism.
- **Retention risk**: repeat rate for new customer cohorts fell from 90.8% (March) to 60.9% (April), signaling a need for early re-engagement campaigns.

## Tools Used

- **Microsoft Excel** — data entry, cleaning, pivot tables, ABC/Pareto, visualization
- **Python** (Pandas, NumPy, Matplotlib, SciPy) — cleaning, feature derivation, hypothesis testing, correlation, cohort/tier segmentation
- **Stata** — descriptive statistics, correlation, time-series plots (mid-term)

## Deliverables

- Proposal Report
- Mid-Term Report (descriptive statistics, correlation, preliminary EDA)
- Final Report (ABC classification, demand-grid, cohort analysis, recommendations)

## Author

Arun Sankar E K 

BS Data Science and Applications, IIT Madras
