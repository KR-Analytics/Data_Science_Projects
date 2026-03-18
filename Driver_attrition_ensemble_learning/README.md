# 🚖 Driver Attrition Prediction (Ride-Hailing Platform)

## Problem Statement
Predicting driver attrition using ensemble learning to enable proactive retention strategies in a ride-hailing platform.

---
## Key Result
Achieved **ROC-AUC ~0.84** using Gradient Boosting to predict driver attrition.

---
## Approach

- Data preprocessing (KNN Imputation, date handling)
- Feature engineering (income & rating trends)
- Class imbalance handling (SMOTE)
- Ensemble models (Random Forest, Gradient Boosting)

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

Ensemble learning models effectively predict driver attrition, enabling data-driven decision-making to improve retention and reduce operational costs. This project demonstrates how machine learning can directly drive business decisions and reduce operational costs.

---
