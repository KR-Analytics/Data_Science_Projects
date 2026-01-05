# Netflix Business Case Study — Content Strategy & Market Insights

## Overview
This project analyzes Netflix’s global content catalog to understand content mix, geographic distribution, genre preferences, and growth patterns. The objective is to identify strategic opportunities for content production, acquisition, and regional expansion using data-driven insights.

---

## Problem Statement
Netflix must continuously decide:
- what type of content to produce (movies vs TV shows),
- which genres to prioritize,
- and which regions offer future growth potential.

This analysis supports those decisions using exploratory data analysis.

---

## Dataset
- Total titles: 8,807  
- Content types: Movies and TV Shows  
- Countries represented: 120+ (after splitting multi-country entries)  
- Key variables include:
  - type (movie / TV show)
  - country
  - genre
  - director
  - date added
  - release year
  - rating
  - duration (minutes or seasons)

---

## Tools Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  

---

## Key Findings

### Content Mix
- Movies account for roughly 70% of the catalog.
- TV shows contribute about 30%.
- This suggests scope for expanding serialized content to improve engagement and retention.

---

### Country-wise Distribution
- Content contribution follows a highly skewed distribution.
- The United States, India, the United Kingdom, Japan, and South Korea dominate the catalog.
- More than 70 countries have fewer than 10 titles, indicating under-represented markets.

---

### Genre Distribution
- The dataset contains 42 unique genres.
- A small set of genres (International Movies, Dramas, Comedies, Documentaries, International TV Shows) dominates the catalog.
- The top 25 genres contribute approximately 93% of all titles.

---

### Director Contribution
- Most directors appear only once in the dataset.
- A very small number of directors contribute multiple titles.
- This highlights potential value in forming long-term partnerships with high-performing creators.

---

### Time-based Trends
- Content additions increased steadily until 2019.
- A decline is observed during 2020–2021, likely due to pandemic-related disruptions.
- Monthly additions show seasonal patterns, with certain months consistently seeing higher releases.

---

### Release Year Analysis
- The majority of titles were released after the year 2000.
- Content concentration peaks in the 2010s.
- Very limited content exists from pre-1980 periods.

---

### Ratings Analysis
- The most common ratings are TV-MA, TV-14, and R.
- This indicates a strong focus on mature and young-adult audiences.

---

### Duration Patterns
- Movie durations peak around 90 minutes.
- Most TV shows have only one season.
- This suggests an opportunity to invest in longer-running series.

---

## Business Recommendations
- Increase investment in TV shows to improve long-term engagement.
- Expand content sourcing in under-represented countries.
- Continue prioritizing high-performing genres.
- Develop exclusive or repeat partnerships with proven directors.
- Improve metadata quality and standardization processes.

---

## Files in This Folder
- `NETFLIX_BCS.ipynb` — exploratory data analysis and visualizations  
- `NETFLIX_BCS.pdf` — detailed business case study  

---

## Conclusion
The analysis shows that Netflix’s catalog is highly concentrated by content type, geography, and genre. Strategic diversification across regions, greater emphasis on TV shows, and stronger creator partnerships can help Netflix sustain growth in a competitive streaming market.
