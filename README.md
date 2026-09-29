# 📊 Sales Performance Analysis

An end-to-end sales analysis project covering **100,000 sales orders** from **January 1 to September 10, 2024**.

The project combines **Python-based data cleaning and analysis** with an interactive **Power BI dashboard** to turn raw sales data into meaningful business insights.

---

## 🚀 Power BI Dashboard

![Sales Dashboard](sales_dashboard_00.png)

---

## 📌 Project Overview

The objective of this project was to analyze sales performance, understand revenue patterns, evaluate discounts, compare product categories, and identify customer and time-based trends.

The workflow followed:

**Raw Data → Data Cleaning → Exploratory Analysis → Business Insights → Power BI Dashboard**

---

## 📈 Key Numbers

| Metric | Value |
|---|---:|
| Original Orders | 100,000 |
| Clean Orders | 90,000 |
| Rows Removed | 10,000 |
| Gross Revenue | $49.5M |
| Net Revenue | $37.2M |
| Discount Cost | $12.3M |
| Discount Rate | 24.9% |
| Average Order Value | $550.17 |

---

## 🎯 Business Questions

The analysis focused on the following questions:

1. What are the gross and net revenues, and how much revenue is lost through discounts?
2. How does revenue change over time?
3. Which product categories generate the most revenue?
4. Do larger discounts lead to larger orders?
5. Do customer age and gender relate to order value?
6. Are there stronger sales days or periods within the month?
7. Is revenue heavily concentrated in a small number of categories?

---

## 🔎 Key Findings

| Finding | Evidence | Confidence |
|---|---|---|
| Discounts do not appear to increase order value | Correlation: **-0.0003** across 90,000 orders | Strong |
| Revenue is distributed relatively evenly across categories | Top 5 categories represent **21.3%** vs. 20.8% for an equal split | Strong |
| Revenue remains relatively stable month to month | Approximately **4%** spread across the 9-month period | Preliminary |
| No category clearly dominates revenue | Approximately **6.7%** gap between the highest and lowest category | Preliminary |
| Customer segments show similar order values | Less than **1%** difference across age and gender groups | Preliminary |

### Confidence Notes

**Strong** findings are supported by a formal statistical measure or a clear difference based on the available sample.

**Preliminary** findings represent observed patterns that would benefit from additional statistical testing such as ANOVA or t-tests.

---

## 🧹 Data Cleaning & Validation

The dataset was cleaned and validated before analysis.

### Main Cleaning Steps

- Removed **10,000 rows (10%)** with missing values.
- Missing values occurred in `Sales_Amount`, `Discount`, `Customer_Age`, and `Customer_Gender`.
- The missing values occurred in the same rows.
- A chi-square test indicated that missingness was not significantly related to:
  - Month (**p = 0.73**)
  - Product Category (**p = 0.50**)
- No duplicate rows were identified.
- `Sales_ID` was unique across the dataset.
- `Discount` was treated as a percentage ranging from **0–50**.
- High-cardinality fields such as `Sales_Region` and `Sales_Representative` were excluded from grouped analysis.

---

## 💡 Business Insights

### Discounts

The correlation between discount percentage and order value was approximately **-0.0003**, indicating virtually no linear relationship in this dataset.

### Product Categories

Revenue was relatively evenly distributed across categories, with no single category accounting for a dominant share of total revenue.

### Customer Segments

Order values were broadly similar across age and gender groups, with differences of less than 1%.

### Revenue Over Time

Monthly revenue remained relatively stable throughout the analyzed period, with approximately a 4% spread between the months.

---

## ⚠️ Limitations

- Some monthly and category revenue figures were carried over from earlier reporting and were not recomputed from raw rows during the final review.
- `Discount` is assumed to represent a percentage. If it represents an absolute amount, net-revenue calculations would need to be recalculated.
- The dataset contains revenue information but does not contain cost or profit data.
- There is no repeat-purchase or customer lifetime data.
- ANOVA and t-tests for the preliminary findings were planned but were not included in the final analysis.
- The dataset represents a specific period from **January 1 to September 10, 2024**, so the findings should not automatically be generalized to other periods.

---

## 🛠️ Tools & Technologies

- **Python**
- **Pandas**
- **NumPy**
- **SciPy**
- **Matplotlib**
- **Seaborn**
- **Power BI**
- **GitHub**

---

## 📂 Repository Contents

| File | Description |
|---|---|
| `sales_analysis0` | Sales analysis work |
| `Sales_Analysis_Presentation.pptx` | Project presentation |
| `sales_dashboard_00.png` | Power BI dashboard |
| `README.md` | Project documentation |

---

## 📊 Project Deliverables

### Power BI Dashboard

The dashboard provides a visual overview of:

- Revenue performance
- Gross vs. net revenue
- Discounts
- Category performance
- Customer segments
- Time-based sales patterns

### Project Presentation

A complete presentation summarizing the analysis, findings, and business insights is available here:

**[View Sales Analysis Presentation](Sales_Analysis_Presentation.pptx)**

---

## 📁 Dataset

The original dataset contains **100,000 sales orders** covering the period from **January 1 to September 10, 2024**.

The raw dataset is not included in this repository.

---

## 👤 Project

**Sales Performance Analysis**

Built as a portfolio project demonstrating an end-to-end **Data Analysis workflow using Python and Power BI**.
