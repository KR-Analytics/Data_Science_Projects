# Walmart Black Friday Purchase Analysis

## Overview
This project analyzes customer purchase behavior during Walmart’s Black Friday sales event. The goal is to understand how spending varies across different customer segments and to identify which demographic factors meaningfully influence purchase amounts.

The analysis focuses on gender, marital status, age groups, and city categories, using both exploratory data analysis and statistical inference to support business decision-making.

---

## Problem Statement
Walmart wants to optimize marketing strategies, promotions, and inventory planning during large sales events such as Black Friday. To do this effectively, it is important to understand:
- whether spending differs meaningfully across genders,
- how marital status affects purchase behavior,
- which age groups contribute the most to revenue,
- and which customer segments should be prioritized for targeted campaigns.

---

## Dataset
- Number of records: ~550,000 transactions  
- Customers: Male and female shoppers across multiple cities  
- Key variables:
  - Gender
  - Age group
  - Marital status
  - City category
  - Occupation
  - Product category
  - Purchase amount

The dataset contains no missing values or duplicate records.

---

## Tools Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- SciPy (statistical testing)

---

## Data Preparation
- Converted categorical variables to appropriate categorical data types
- Ordered age groups to reflect life stages rather than alphabetical order
- Verified data quality (no null values, no duplicates)
- Optimized memory usage for large-scale analysis

---

## Key Findings

### Overall Customer Profile
- Around 60% of customers fall in the 26–45 age range, indicating dominance of young and mid-career adults.
- City Category B contributes the largest share of customers.
- Approximately 75% of the customer base is male.
- Around 60% of customers are unmarried.

---

### Purchase Distribution
- Purchase amounts are right-skewed with a small number of high-value outliers.
- The majority of transactions fall within a moderate spending range.
- Outliers account for less than 1% of total observations.

---

### Gender-wise Analysis
- Average purchase amount for males is higher than for females.
- Sampling distributions of mean purchase values closely match population means.
- Confidence intervals for male and female spending do not fully overlap.
- An independent samples t-test shows that gender has a statistically significant impact on purchase amount.

---

### Marital Status Analysis
- Mean purchase amounts for married and unmarried customers are nearly identical.
- Confidence intervals for both groups overlap substantially.
- Statistical testing fails to reject the null hypothesis.
- Marital status does not have a significant impact on purchase amount.

---

### Age-wise Analysis
- The largest customer group is 26–35 years, followed by 18–25 years.
- Average spending increases with age and peaks in the 51–55 age group.
- Variability in spending is similar across age groups.
- One-way ANOVA confirms that age has a statistically s

## Conclusion
This analysis highlights that **age and gender play a meaningful role in determining purchase behavior during Black Friday**, while marital status has minimal influence. Understanding these patterns allows Walmart to design more targeted promotions, allocate inventory more efficiently, and focus marketing efforts on customer segments with higher spending potential. Applying these insights can help improve both customer engagement and revenue outcomes during large-scale sales events.
