# Admission Prediction using Linear Regression

## Author  
Radhika Agrawal  
Data Analyst | Business & Performance Analytics | SQL | Python | Power BI | Regression Modeling  

---

## Project Overview

This project analyzes applicant profiles to predict the probability of admission to top foreign universities. Historical admission data was used to identify academic and profile-related factors influencing admission outcomes through regression-based modeling.

The work demonstrates an end-to-end analytical workflow, including data validation, exploratory analysis, statistical modeling, and business interpretation.

---

## Objectives

- Identify key drivers of admission probability  
- Perform structured exploratory data analysis  
- Build and validate a Linear Regression model  
- Test statistical assumptions and model stability  
- Translate analytical findings into practical insights  

---

## Dataset

**Source:** Jamboree Admission Dataset  
**Records:** 500 applicants  

**Features:**
- GRE Score  
- TOEFL Score  
- CGPA  
- University Rating  
- SOP  
- LOR  
- Research Experience  

**Target Variable:**
- Chance of Admit  

---

## Tools and Technologies

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Statsmodels  
- Scikit-learn  

---

## Methodology

### Data Preparation
- Removed non-informative identifiers  
- Standardized column names  
- Checked for missing values  
- Verified data types and consistency  

### Exploratory Data Analysis
- Univariate and bivariate analysis  
- Correlation assessment  
- Distribution analysis  

### Model Development
- Train-test split (80:20)  
- OLS regression using Statsmodels  
- Multicollinearity analysis using VIF  
- Residual diagnostics  

### Regularization
- Ridge regression  
- Lasso regression  
- Coefficient comparison  

### Model Evaluation
- R² and Adjusted R²  
- RMSE and MAE  
- Train vs test performance analysis  

---

## Results

- Test R² ≈ 0.83  
- Adjusted R² ≈ 0.81  
- Strongest predictors: CGPA, GRE, TOEFL, LOR, Research  
- Model demonstrates good generalization  

---

## Key Insights

- CGPA is the strongest predictor of admission probability  
- Standardized test scores have significant influence  
- Research experience improves outcomes  
- SOP has limited impact when academic metrics are strong  
- LOR remains a consistent contributor  

---

## Business Recommendations

- Applicants should focus on academic performance and research exposure  
- Institutions can use predictive models for preliminary screening  
- Counseling services can provide data-driven guidance  
- The model can support admission evaluation workflows  

---

## Future Enhancements

- Cross-validation for robustness  
- Model deployment using Streamlit  
- Feature engineering  
- Web interface integration  

---

## Repository Contents

- Analysis notebook / PDF  
- Visualizations  
- Model evaluation results  
- Documentation  

---

## Contact

Details available in profile (GitHub / LinkedIn)
