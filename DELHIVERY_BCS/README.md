# 🚚 Delhivery Business Case Study — Logistics Data Analysis & Insights

## 📌 Overview
This project analyzes large-scale logistics and routing data from **Delhivery**, a nationwide supply-chain and last-mile delivery company. The objective is to evaluate **actual delivery performance versus OSRM-based routing estimates**, identify delay patterns, and derive operational insights that can improve planning accuracy and efficiency.

The analysis works at **segment-level and trip-level granularity**, transforming raw operational logs into analysis-ready datasets suitable for forecasting and optimization.

---

## 🎯 Problem Statement
Routing engines such as OSRM provide ideal travel time and distance estimates, but **real-world delivery performance often deviates** due to traffic, hub delays, route segmentation, and operational constraints.

This project aims to:
- Clean and structure raw logistics data
- Engineer meaningful trip- and segment-level features
- Quantify delays and inefficiencies
- Compare actual vs predicted (OSRM) performance
- Identify consistently underperforming routes and hubs
- Support future delivery-time forecasting models

---

## 📊 Dataset
- **Records:** ~145,000 shipment-level observations
- **Granularity:** Segment-level logs aggregated to trip-level
- **Key variables:**
  - Trip and segment timestamps
  - Actual time and distance
  - OSRM-predicted time and distance
  - Route type (FTL vs Carting)
  - Source and destination hubs
  - Scan-to-scan duration

Missing source and destination names were systematically resolved using ID–name mappings.

---

## 🧰 Tools & Libraries
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- SciPy (statistical testing)  
- scikit-learn (scaling & preprocessing)

---

## 🧹 Data Preparation & Feature Engineering
- Datetime parsing and safe coercion
- Numeric type casting for performance
- Memory optimization using categorical dtypes
- Segment-level aggregation → Trip-level aggregation
- Feature creation:
  - Trip duration (hours & minutes)
  - Delay and delay ratio
  - Average speed (km/h)
  - OSRM vs actual performance metrics
- Outlier detection using IQR
- One-hot encoding of categorical variables
- Standardization of numerical features

---

## 🔬 Statistical Analysis & Hypothesis Testing

### Key Comparisons
- **Trip duration vs scan-to-scan time**
- **Actual time vs OSRM-predicted time**
- **Trip-level vs segment-aggregated time**
- **Trip-level vs segment-aggregated distance**

Both **paired t-tests** and **Wilcoxon signed-rank tests** were used, along with effect size (Cohen’s d), to ensure robustness.

---

## 🔍 Key Insights

1. **Actual delivery times consistently exceed OSRM predictions**  
   OSRM underestimates both time and distance across most trips, highlighting real-world operational delays.

2. **Segment-level aggregation inflates time and distance**  
   Summing over multiple segments produces higher totals than trip-level estimates, indicating inefficiencies from multi-hop routing.

3. **Major delays occur before physical movement begins**  
   Trip duration is far greater than scan-to-scan time, showing that sorting, loading, queueing, and handover dominate delays.

4. **Route type matters**  
   - **FTL routes** are faster and more consistent  
   - **Carting routes** show higher variability and longer delays

5. **Corridor-specific inefficiencies exist**  
   Certain source–destination pairs repeatedly underperform, suggesting localized traffic or hub bottlenecks.

6. **Distance strongly correlates with time**  
   Longer corridors consistently take longer than predicted, indicating predictable, scalable delays.

7. **High outliers point to hub-level issues**  
   Some segments exhibit extreme delays, signaling operational problems at specific centers.

---

## 📈 Business Recommendations
- Prioritize optimization of **high-delay corridors**
- Improve **pre-dispatch processes** at busy hubs
- Re-evaluate **route segmentation strategy**
- Add realistic **planning buffers** for high-variance routes
- Optimize **carting route design and fleet allocation**
- Prefer **FTL routing** where feasible
- Conduct audits at hubs causing repeated delays
- Enhance OSRM predictions using historical delay factors
- Reduce unnecessary scans and micro-stops
- Focus resources on **high-volume hubs** for maximum impact

---

## 📁 Files in This Folder
- `DELHIVERY_BCS.ipynb` — Complete data cleaning, feature engineering, EDA, and hypothesis testing  
- `DELHIVERY_BCS.pdf` — Detailed business case study and visual analysis  

---

## 🧠 Conclusion
The analysis shows that **actual delivery performance is systematically slower and more variable than OSRM predictions**. Segment-level aggregation further amplifies these gaps, revealing structural inefficiencies in routing and hub operations. Incorporating real-world delay patterns into planning and focusing on high-impact corridors and hubs can significantly improve delivery reliability and ETA accuracy.
