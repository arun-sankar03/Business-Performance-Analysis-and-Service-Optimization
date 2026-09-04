# Business-Performance-Analysis-and-Service-Optimization

### A Primary Data Study of a Professional Laundry Business

This project was completed as part of the **Business Data Management (BDM) Capstone Project** for the **BS Degree in Data Science and Applications, IIT Madras**.

The study analyses the business performance of **RDS Associates**, operating under the trade name **Rinz n Dry**, a B2C laundry and dry-cleaning business located in Thrissur, Kerala.

The project uses **2,607 primary customer order records** collected directly from the business between **10 March 2026 and 10 July 2026**, covering **106 working days**. The analysis focuses on service demand, revenue contribution, operational efficiency, turnaround time, complaints, and customer retention.

---

## Project Objectives

The analysis addresses three major business problems:

1. **Revenue and Service Demand Imbalance**

   * Identify services contributing most to revenue.
   * Compare service demand with revenue contribution.
   * Examine revenue efficiency at the garment level.
   * Understand service preference across new and regular customers.

2. **Operational Efficiency and Turnaround Time**

   * Analyse turnaround time across service levels and services.
   * Identify high-demand time windows using hour × weekday analysis.
   * Examine complaint trends over the study period.
   * Evaluate the role of Express services and delivery charges.

3. **Customer Retention and Behavioural Patterns**

   * Analyse repeat-purchase behaviour.
   * Measure revenue concentration across customer-frequency tiers.
   * Compare retention across customer acquisition cohorts.
   * Examine the relationship between complaints and subsequent customer visits.

---

## Dataset

The dataset contains customer order-level information including:

* Order Date and Order Time
* Customer ID
* Customer Type
* Type of Service
* Service Level
* Number of Garments
* Bill Amount
* Payment Mode
* Pickup/Delivery Type
* Extra Distance
* Delivery Date
* Turnaround Time
* Complaint Status

The data was collected directly from the organization's digital records and supplemented by operational information obtained through discussion with the business owner. The dataset was cleaned and validated before analysis.

> **Note:** The original customer-level dataset is not intended for public redistribution because it was collected as primary business data for academic analysis.

---

## Methodology

The project followed a structured analytical workflow:

**Data Collection → Data Cleaning → Exploratory Data Analysis → Statistical Analysis → Service Analysis → Operational Analysis → Customer Segmentation → Findings → Recommendations**

### Data Cleaning & Validation

The dataset was checked for:

* Duplicate records
* Missing values
* Date and range consistency
* Outliers
* Date-time conversion
* Aggregate-level cross-validation with business records

No duplicate records were identified, core operational fields contained no missing values, and unusual observations outside the IQR were confirmed as genuine bulk transactions rather than data-entry errors.

### Analytical Methods

The project used:

* Descriptive statistics
* Exploratory Data Analysis (EDA)
* Service-wise tabulation
* Independent two-sample t-test
* Chi-square test
* One-way ANOVA
* Pearson correlation analysis
* Weekly time-series analysis
* ABC/Pareto classification
* Revenue-per-garment analysis
* Hour × weekday demand grid
* Customer order-frequency segmentation
* Acquisition cohort analysis
* Complaint and repeat-behaviour analysis

The later-stage analysis extended the earlier descriptive analysis using revenue concentration, pricing efficiency, service-level comparison, time-grid analysis, customer tiers, and acquisition cohorts.

---

## Tools & Technologies

### Python

* Pandas
* NumPy
* Matplotlib
* SciPy

Used for data cleaning, preprocessing, variable derivation, statistical testing, correlation analysis, time-based aggregation, segmentation, and visualisation.

### Microsoft Excel

Used for:

* Data organisation
* Cleaning
* Pivot tables
* Descriptive calculations
* Service and customer summaries
* Visualisation

### Stata

Used during the analytical stages for statistical analysis, tabulation, correlation analysis, and preliminary time-series analysis.

---

## Key Findings

### 1. Wash & Iron is the core revenue driver

**Wash & Iron** accounts for:

* **47.8% of total orders**
* **62.9% of total revenue**
* **1,246 orders**
* **₹8,24,685 revenue**

The ABC analysis classifies Wash & Iron as the only **Class A service**, indicating that capacity and resource allocation should prioritise this service.

### 2. Revenue efficiency differs significantly across services

Revenue-per-garment analysis shows substantial differences in pricing efficiency.

* **Blanket Washing:** ₹471/garment
* **Bag Cleaning:** ₹373/garment
* **Wash & Fold:** ₹73/garment
* Dataset average: approximately **₹138/garment**

This indicates a potential pricing or garment-count issue for Wash & Fold despite its relatively high order volume.

### 3. Express service is a premium service

Express orders represent only **11.4% of orders**, but have a substantially higher average bill than Normal orders.

* Normal average bill: **₹472.4**
* Express average bill: **₹739.5**
* Express TAT: **1 day**
* Express TAT standard deviation: **0 days**

The difference in average billing was statistically significant (**t = -11.12, p < 0.001**), supporting Express as a reliable premium service.

### 4. Demand is concentrated in specific day-hour combinations

The demand grid shows that:

* **Wednesday, 9–10 AM:** approximately 87 orders
* **Monday, 10–11 AM:** approximately 82 orders
* **9–10 AM and 5–6 PM:** major recurring peak periods

This suggests that staffing should be adjusted according to specific day-hour combinations rather than distributed uniformly throughout the day.

### 5. Revenue is strongly concentrated among repeat customers

Customers placing **4 or more orders** represent only **21.7% of customers**, but contribute **54.5% of total revenue**.

The **2–3 order segment** contains 259 customers and contributes **24.5% of revenue**, making this group an important target for increasing repeat purchasing.

### 6. Recent customer cohorts show weaker repeat behaviour

The repeat rate declined from:

**March cohort: 90.8% → April: 60.9% → May: 45.2% → June: 16.8%**

However, later cohorts have had less time to return, so comparisons are more reliable between earlier cohorts with sufficient observation periods.

### 7. Complaint resolution may support retention

Overall:

* **14.4% of orders** had complaints.
* **90.7% of complaints** were resolved through rectification, compensation, or refund.

Among the March–April acquisition cohort, customers who complained during their first order showed a higher subsequent return rate than customers without a first-order complaint. A chi-square test found this difference to be statistically significant (**χ² = 44.21, p < 0.001**).

---

## Business Recommendations

Based on the analysis, the project recommends:

### Capacity & Pricing

* Prioritise staff and machine capacity for **Wash & Iron**.
* Review the pricing or garment-count structure of **Wash & Fold**.
* Treat Class B services as monitoring priorities and Class C services as lower-priority capacity areas.

### Operations

* Allocate additional resources during peak periods, particularly **Monday and Wednesday mornings**.
* Promote the **Express service** more effectively as a reliable premium offering.
* Review operational changes associated with the rise in complaints between May and June.

### Customer Retention

* Focus retention efforts on customers in the **2–3 order tier** and encourage progression toward 4–6 orders.
* Use WhatsApp/SMS reminders to encourage customers to return within approximately **15–21 days**.
* Maintain and formalise the complaint-resolution process as part of the customer experience.

### Customer Feedback

A structured feedback mechanism was also proposed to capture:

* Overall satisfaction
* TAT reliability
* Service-specific feedback
* Improvement suggestions
* Recommendation likelihood

These strategic recommendations are intended to complement, rather than replace, the findings directly supported by the dataset.

---

## Project Limitations

The study covers approximately four months of business activity. Therefore, the findings are useful for analysing short-run business behaviour and operational performance but are not sufficient to establish annual or seasonal patterns. A longer dataset would allow stronger seasonal and longitudinal analysis.

---

## Project Outcome

The project demonstrates how primary business data can be transformed into actionable insights using statistical analysis, exploratory data analysis, customer segmentation, and service-level analysis.

The findings provide a data-driven basis for:

* Resource allocation
* Service prioritisation
* Pricing review
* Operational planning
* Customer retention
* Complaint management

---

## Author

**Arun Sankar E K**

BS in Data Science and Applications,


Indian Institute of Technology Madras

**Project:** BDM Capstone Project
**Term:** May 2026

---

## Disclaimer

This repository was created for **academic and portfolio purposes**. The analysis is based on primary business data collected with organizational permission. Business-sensitive or personally identifiable customer information should not be redistributed without appropriate authorization.
