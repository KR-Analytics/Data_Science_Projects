# Loan Default Prediction using Logistic Regression

## Project Overview
This project focuses on building a data-driven credit risk assessment model for **LoanTap**, an online lending platform. The objective is to predict whether a borrower is likely to **fully repay** or **default** on a loan using demographic, financial, employment, and credit history data.

A Logistic Regression model was developed to support underwriting decisions and help reduce Non-Performing Assets (NPAs).

---

## Business Objective
- Analyze borrower behavior using Exploratory Data Analysis (EDA)
- Identify key drivers of loan default
- Build a predictive classification model
- Evaluate model performance using appropriate metrics
- Provide actionable business recommendations

---

## Dataset
- Total Records: ~396,000
- Features: 27
- Target Variable: `loan_status` (Fully Paid / Charged Off)

Data includes:
- Loan details
- Income & employment data
- Credit history
- Debt and utilization metrics

---

## Exploratory Data Analysis (EDA)
Key insights from EDA:

- Most loans range between ₹8,000–₹20,000
- Interest rates are higher for risky borrowers
- Income and DTI show heavy right-skewness
- Moderate class imbalance (≈80% Fully Paid, 20% Charged Off)
- Grades B and C dominate the portfolio
- Debt consolidation is the most common loan purpose

Outliers were detected in:
- Annual income
- DTI
- Revolving balance
- Revolving utilization

These were treated using percentile capping.

---

## Data Preprocessing
Steps performed:

- Missing value imputation (mode / median)
- Outlier treatment (1st–99th percentile capping)
- Feature engineering (risk flags)
- Categorical encoding (One-Hot Encoding)
- Feature scaling (StandardScaler)
- Stratified Train-Test Split (80:20)

Removed non-predictive features:
- Address
- Employment title
- Issue date
- Credit line dates

---

## Feature Engineering
New features created:

- Public record risk flag
- Mortgage account flag
- Bankruptcy flag

These indicators helped capture high-risk borrower behavior.

---

## Model Development
Algorithm Used:
- Logistic Regression (Scikit-learn)

Key Settings:
- Class weight balancing
- Max iterations: 1000
- Standardized inputs

Target Encoding:
- Fully Paid → 0
- Charged Off → 1

---

## Model Evaluation

### Confusion Matrix Insights
- Strong performance on non-defaulters
- High false negatives for defaulters
- Conservative prediction behavior

### Classification Report (Summary)
- Accuracy: ~65%
- Defaulter Recall: Low
- Non-defaulter Recall: High
- F1-score: Moderate

### ROC-AUC
- AUC ≈ 0.71
- Indicates reasonable discriminatory power

### Key Observations
- Accuracy is inflated due to class imbalance
- Default detection needs improvement
- Threshold tuning is required

---

## Important Risk Drivers
Top influential features:

- Loan grade (C–F)
- Sub-grade (C3–D5)
- Interest rate
- DTI ratio
- Income stability
- Revolving utilization

These variables strongly affect default probability.

---

## Business Insights & Recommendations

### Risk Management
- Prioritize Recall over Accuracy
- Apply stricter approval for high-risk profiles
- Introduce risk-based pricing
- Enforce stronger income verification
- Limit exposure for high DTI borrowers

### Operational Improvements
- Lower probability threshold
- Use cost-sensitive learning
- Combine ML with manual review
- Retrain model periodically

### Strategic Benefits
- Reduced NPAs
- Improved portfolio quality
- Better credit allocation
- Enhanced underwriting decisions

---

## Tech Stack
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Google Colab

---

## Future Enhancements
- Apply SMOTE for class imbalance
- Try ensemble models (XGBoost, Random Forest)
- Perform hyperparameter tuning
- Implement cost-sensitive classification
- Deploy as credit risk scoring tool

---

## Author
**Radhika Agrawal**  
Data Analyst | AI/ML Practitioner  
Regression Modeling | Predictive & Business Analytics  

**Skills**: Python, SQL, Excel, Power BI, Statistics, Regression Analysis, Machine Learning, Financial Analytics

---
## Contact
For collaboration or feedback, feel free to connect via LinkedIn.
