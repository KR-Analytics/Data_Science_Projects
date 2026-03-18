# 🚖 Driver Attrition Prediction (Ride-Hailing Platform)

## Problem Statement
Driver attrition is a major challenge for ride-hailing platforms. This project aims to predict whether a driver is likely to leave the platform using historical data on demographics, tenure, and performance.

---

## Approach

### Data Preprocessing
- Date feature transformation
- Handling missing values using KNN Imputation
- Aggregation from monthly level to driver level

### Feature Engineering
- Income trend (increase/decrease)
- Rating trend (increase/decrease)
- Target variable creation (attrition)

### Handling Class Imbalance
- Applied SMOTE to balance minority class

---

## Models Used

### Random Forest (Bagging)
- Reduces variance using multiple decision trees

### Gradient Boosting (Boosting)
- Improves performance by focusing on misclassified cases

---

## Results

| Model              | Accuracy | ROC-AUC |
|-------------------|---------|--------|
| Random Forest     | ~82%    | 0.836  |
| Gradient Boosting | ~81%    | 0.837  |

---

## Key Insights

- Drivers with **low income** are more likely to leave  
- Drivers with **low ratings (especially rating = 1)** have high attrition  
- Drivers with **low business value contribution** are at higher risk  
- Performance-related factors are stronger predictors than demographics  

---

## Business Recommendations

- **INCOME STABILIZATION** – Reduce income volatility  
- **PERFORMANCE INCENTIVES** – Reward consistent performers  
- **EARLY WARNING SYSTEM** – Identify at-risk drivers proactively  
- **CITY-LEVEL STRATEGY** – Address location-based challenges  
- **FOCUS ON LOW PERFORMERS** – Improve performance via training & feedback  

---

## Tech Stack

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Imbalanced-learn  

---

## Files

- `ola_driver_analysis.ipynb` → Complete notebook  
- `report.pdf` → Summary report (if uploaded)

---

## Conclusion

Ensemble learning models effectively predict driver attrition, enabling data-driven decision-making to improve retention and reduce operational costs.

---
