# Scaler Business Case Study: Learner Segmentation using Clustering

## Project Overview

This project analyzes **205,687 learner records** from Scaler to understand compensation patterns across companies, job roles, and experience levels. The objective is to profile learners through both **manual clustering** and **unsupervised machine learning**, enabling meaningful salary benchmarking and learner segmentation.

The analysis combines Exploratory Data Analysis (EDA), feature engineering, business-driven clustering, and machine learning techniques to generate actionable insights that can support career guidance, salary benchmarking, and strategic decision-making.

---

## Business Problem

Scaler aims to profile learners based on their **current company**, **job position**, **work experience**, and **CTC (Compensation)** to answer business questions such as:

- Which companies offer the highest compensation?
- Which job roles are the highest paying?
- Which employees earn above or below their peer groups?
- Can learners be segmented into meaningful career clusters?
- How can these insights improve learner guidance and placement strategies?

---

## Dataset Information

- **Source:** Scaler Business Case Study
- **Records:** **205,687**
- **Features:** **7**

### Dataset Features

| Feature | Description |
|----------|-------------|
| company_hash | Anonymized company identifier |
| email_hash | Anonymized learner identifier |
| orgyear | Employment start year |
| ctc | Current annual compensation |
| job_position | Current job role |
| ctc_updated_year | Year of latest CTC update |

---

# Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy

---

# Project Workflow

```
Data Loading
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Data Cleaning
      │
      ▼
Feature Engineering
      │
      ▼
Manual Clustering
(Designation • Class • Tier)
      │
      ▼
Business Analysis
      │
      ▼
Label Encoding
      │
      ▼
Standardization
      │
      ▼
Hopkins Statistic
      │
      ▼
Elbow Method
      │
      ▼
K-Means Clustering
      │
      ▼
Hierarchical Clustering
      │
      ▼
Business Insights & Recommendations
```

---

# Exploratory Data Analysis

The analysis included:

- Dataset overview
- Missing value analysis
- Duplicate detection
- Unique learner analysis
- Statistical summaries
- Distribution analysis
- Outlier detection
- Feature engineering

---

# Feature Engineering

A new feature was created:

- **Years_of_Experience = Current Year − Organization Joining Year**

This enabled experience-based salary benchmarking throughout the analysis.

---

# Manual Clustering

Three business-driven clustering strategies were developed.

### Designation

Salary comparison within:

- Company
- Job Position
- Years of Experience

### Class

Salary comparison within:

- Company
- Job Position

### Tier

Salary comparison within:

- Company

These classifications enabled identification of employees earning above or below their respective peer groups.

---

# Unsupervised Learning

The following clustering techniques were implemented:

- Label Encoding
- Feature Standardization
- Hopkins Statistic
- Elbow Method
- K-Means Clustering
- Hierarchical Clustering

The Hopkins Statistic confirmed a strong clustering tendency, while the Elbow Method identified the optimal number of clusters for K-Means.

---

# Key Business Insights

- Salary benchmarking is more meaningful when employees are compared within the same company, role, and experience level.
- Mid-career professionals (5–7 years of experience) form an important learner segment.
- Significant salary variation exists across companies for similar job roles.
- K-Means successfully segmented learners into distinct compensation and experience groups.
- Hierarchical Clustering validated the segmentation identified through K-Means.
- The analysis highlights organizations offering competitive compensation and identifies potential salary disparities.

---

# Business Recommendations

- Implement peer-group salary benchmarking.
- Recommend high-paying companies based on historical compensation trends.
- Personalize learner guidance using cluster membership.
- Identify underpaid learner segments for targeted career support.
- Strengthen placement partnerships with consistently high-paying organizations.
- Continuously monitor salary trends to improve learner recommendations.

---

# Future Improvements

- Apply PCA for cluster visualization.
- Evaluate cluster quality using Silhouette Score.
- Compare K-Means with DBSCAN and Gaussian Mixture Models.
- Build an interactive dashboard using Power BI or Tableau.
- Deploy the analysis as a Streamlit web application.

---

# Connect With Me

If you found this project interesting, feel free to connect!

- **LinkedIn:** www.linkedin.com/in/kradhika444/
- **GitHub:** https://github.com/KR-Analytics

---
