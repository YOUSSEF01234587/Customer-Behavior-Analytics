# Customer Behavior Analytics

### Turning Retail Data into Actionable Business Insights

**Prepared by:** Youssef Talaat  
**Project Type:** End-to-End Data Analytics  
**Tools:** Python · SQL · PostgreSQL · Power BI

---

## 📌 Project Overview

This project analyzes **3,900 retail shopping records** to explore purchasing patterns, product performance, customer demographics, discount usage, shipping preferences, and customer ratings.

The workflow combines Python-based data preparation, PostgreSQL storage, SQL analysis, and an interactive Power BI dashboard to transform raw data into actionable business insights and practical recommendations.

## 🎯 Business Problem

The business aims to better understand customer shopping behavior to support sales performance, customer satisfaction, customer engagement, inventory planning, and marketing decisions.

This analysis investigates how recorded purchase value and purchasing patterns vary across demographic groups, product categories, discount status, shipping types, seasons, and subscription status.

## 📊 Key Results

| Metric | Result |
|---|---:|
| Purchase Records | 3,900 |
| Total Recorded Purchase Value | $233,081 |
| Average Purchase Amount | $59.76 |
| Average Review Rating | 3.75 / 5 |
| Records with a Discount | 1,677 |
| Discount Rate | 43.0% |
| Missing Review Ratings Identified and Imputed | 37 |
| Original Dataset Columns | 18 |

> **Interpretation Note:** Recorded purchase value is not equivalent to profit or verified net revenue. The dataset does not include product costs, returns, or margin data.

## 🔄 Analytics Workflow

### 1. Data Preparation — Python

- Inspected and cleaned the dataset.
- Identified and imputed 37 missing review ratings using category-level medians.
- Standardized column names.
- Created age groups.
- Converted purchase-frequency categories into approximate day intervals.
- Removed a redundant promotional-code field after a consistency check.

### 2. Database — PostgreSQL

- Loaded the prepared dataset into the `customer` table.
- Used the `customer_behavior` database for structured analysis.

### 3. SQL Analysis

- Analyzed purchase value by gender and age group.
- Examined product ratings and shipping preferences.
- Investigated discount patterns and customer-history segments.
- Ranked products using analytical queries.

### 4. Power BI Dashboard

Created five interactive dashboard pages:

- Landing Page
- Overview Dashboard
- Customer Analysis
- Product Analysis
- Discount Analysis

### 5. Business Recommendations

Identified opportunities to improve reporting reliability, inventory planning, promotional evaluation, customer engagement, and shipping strategies.

## 🔍 Selected Findings

### 1. Customer Demographics

#### Recorded Purchase Value by Gender

| Gender | Recorded Purchase Value | Share |
|---|---:|---:|
| Male | $157,890 | 67.74% |
| Female | $75,191 | 32.26% |

Male-associated records account for 67.74% of the recorded purchase value. This descriptive difference does not establish the reasons behind the difference.

#### Recorded Purchase Value by Age Group

| Age Group | Recorded Purchase Value |
|---|---:|
| Young Adults | $62,143 |
| Middle-aged | $59,197 |
| Adult | $55,978 |
| Senior | $55,763 |

Young Adults have the highest recorded purchase value among the reported age groups.

### 2. Product Category Performance

| Category | Purchase Records | Share |
|---|---:|---:|
| Clothing | 1,737 | 44.54% |
| Accessories | 1,240 | 31.79% |
| Footwear | 599 | 15.36% |
| Outerwear | 324 | 8.31% |

**Key Insight:** Clothing and Accessories together account for **76.33% of purchase records**. These categories deserve attention when analyzing demand and planning inventory.

### 3. Shipping Analysis

| Shipping Type | Average Purchase Amount |
|---|---:|
| Express | $60.48 |
| Standard | $58.46 |
| Difference | $2.02 |

Express-shipping records have an average purchase amount $2.02 higher than Standard-shipping records.

This is an observed association and does not prove that Express shipping causes higher spending.

### 4. Discount Analysis

| Metric | Result |
|---|---:|
| Records Using a Discount | 1,677 |
| Discount Rate | 43.0% |
| Average Purchase Amount with Discount | $59.28 |
| Average Purchase Amount without Discount | $60.13 |

The average purchase amount is slightly lower for discounted records. This difference alone cannot determine whether discounts increase conversion or reduce profitability.

### 5. Highest Reported Average Product Ratings

| Rank | Product | Average Rating |
|---:|---|---:|
| 1 | Gloves | 3.86 / 5 |
| 2 | Sandals | 3.84 / 5 |
| 3 | Boots | 3.82 / 5 |
| 4 | Hat | 3.80 / 5 |
| 5 | Skirt | 3.78 / 5 |

### 6. Products with the Highest Reported Discount Rates

| Rank | Product | Discount Rate |
|---:|---|---:|
| 1 | Hat | 50.00% |
| 2 | Sneakers | 49.66% |
| 3 | Coat | 49.07% |
| 4 | Sweater | 48.17% |
| 5 | Pants | 47.37% |

These rankings can help prioritize further investigation into product-level promotional activity.

## 💡 Business Recommendations

1. **Validate reporting first:** Reconcile subscription totals between SQL and Power BI, verify the discount-by-gender chart, and confirm whether the records represent unique customers or purchase transactions.

2. **Improve inventory decisions:** Monitor high-volume categories and products, then combine demand data with stock availability, returns, product costs, and gross margin before changing inventory levels.

3. **Measure discount effectiveness:** Compare discounted and non-discounted transactions by product. Test promotional levels against a control group and monitor conversion, average purchase amount, and gross margin.

4. **Develop customer engagement:** Once customer segments are validated, test retention campaigns for established buyers, re-engagement campaigns for returning buyers, and onboarding campaigns for new buyers.

5. **Evaluate shipping options:** Test targeted Express-shipping offers while monitoring shipping costs, delivery performance, customer satisfaction, and contribution margin.

6. **Establish a KPI review routine:** Monitor recorded purchase value, average purchase amount, discount rate, ratings, category share, repeat-purchase rate, gross margin, and stockout rate where supporting data exists.

## 🖥️ Dashboard Screenshots

The following screenshots illustrate the dataset, data preparation, database verification, and Power BI dashboards.

### Figure 1 — Dataset Overview

![Figure 1 — Dataset Overview](Assets/Figure%201%20%E2%80%94%20Dataset%20Overview.png)

### Figure 2 — Data Quality

![Figure 2 — Data Quality](Assets/Figure%202%20%E2%80%94%20Data%20Quality.png)

![Figure 2 — Data Quality 2](Assets/Figure%202%20%E2%80%94%20Data%20Quality2.png)

### Figure 3 — Analytics Workflow

![Figure 3 — Analytics Workflow](Assets/Figure%203%20%E2%80%94%20Analytics%20Workflow.png)

### Figure 4 — Database Verification

![Figure 4 — Database Verification 1](Assets/Figure%204%20%E2%80%94%20Database%20Verification1.png)

![Figure 4 — Database Verification 2](Assets/Figure%204%20%E2%80%94%20Database%20Verification2.png)

### Figure 5 — Landing Page

![Figure 5 — Landing Page](Assets/Figure%205%20%E2%80%94%20Landing%20Page.png)

### Figure 6 — Overview Dashboard

![Figure 6 — Overview Dashboard](Assets/Figure%206%20%E2%80%94%20Overview%20Dashboard.png)

### Figure 7 — Customer Analysis Dashboard

![Figure 7 — Customer Analysis Dashboard](Assets/Figure%207%20%E2%80%94%20Customer%20Analysis%20Dashboard.png)

### Figure 8 — Product Analysis Dashboard

![Figure 8 — Product Analysis Dashboard](Assets/Figure%208%20%E2%80%94%20Product%20Analysis%20Dashboard.png)

### Figure 9 — Discount Analysis Dashboard

![Figure 9 — Discount Analysis Dashboard](Assets/Figure%209%20%E2%80%94%20Discount%20Analysis%20Dashboard.png)

## 📁 Repository Structure

```text
Customer-Behavior-Analytics/
├── Assets/
│   ├── Figure 1 — Dataset Overview.png
│   ├── Figure 2 — Data Quality.png
│   ├── Figure 2 — Data Quality2.png
│   ├── Figure 3 — Analytics Workflow.png
│   ├── Figure 4 — Database Verification1.png
│   ├── Figure 4 — Database Verification2.png
│   ├── Figure 5 — Landing Page.png
│   ├── Figure 6 — Overview Dashboard.png
│   ├── Figure 7 — Customer Analysis Dashboard.png
│   ├── Figure 8 — Product Analysis Dashboard.png
│   └── Figure 9 — Discount Analysis Dashboard.png
├── Data/
│   └── Raw and/or prepared dataset files
├── Database/
│   └── SQL scripts and analytical queries
├── Dynamic Dashboard/
│   └── Power BI report (.pbix)
├── Notebook/
│   └── Python/Jupyter analysis notebook (.ipynb)
├── Business Problem Document.pdf
└── README.md
```

## ⚠️ Data Limitations

- The dataset does not clearly identify online versus offline sales channels.
- Purchase amounts are not equivalent to profit; product costs, returns, and margins were not supplied.
- Differences between groups are descriptive and do not establish causation.
- Subscription figures reported by SQL conflict with the earlier Power BI summary and require reconciliation.
- The discount-by-gender visualization appears inconsistent and must be checked.
- Customer loyalty claims require confirmation that the identifiers and record structure support unique-customer analysis.

These limitations should be resolved before using the findings to make high-impact business decisions.

## 🛠️ Tools and Skills Demonstrated

- **Programming:** Python, pandas
- **Data Preparation:** Data Cleaning, Missing-Value Treatment, Feature Engineering
- **Databases:** PostgreSQL, SQL
- **SQL Analytics:** Aggregations, Grouping, Window Functions
- **Business Intelligence:** Power BI, KPI Reporting, Interactive Dashboards
- **Analytics:** Customer Segmentation, Product Analysis, Discount Analysis
- **Business:** Data Interpretation, Reporting Validation, Business Recommendations

## 👨‍💻 Author

**Youssef Talaat**

AI & Data Analytics · Python · SQL · PostgreSQL · Power BI

---

*Customer Behavior Analytics — Turning Retail Data into Actionable Business Insights.*
