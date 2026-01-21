# 📊 Nashik Aadhaar Enrollment Insights (2025)

## 🧠 Problem Statement
Aadhaar enrollment is a critical pillar of India’s digital identity system. However, enrollment activity is not uniform across time periods, age groups, or geographic regions. Understanding these variations is essential for effective planning, resource allocation, and improving enrollment accessibility.

This project analyzes Aadhaar enrollment data for **Nashik district** to identify:
- Seasonal enrollment trends
- Age-group-wise contribution
- High and low enrollment pincode areas

The objective is to generate **data-driven insights** that can support better decision-making for Aadhaar enrollment initiatives.

---

## 📂 Dataset Description
- **Region:** Nashik District
- **Data Type:** Aadhaar enrollment records
- **Granularity:** Date, pincode, and age group level

### Age Groups Analyzed
- 0–5 years  
- 5–17 years  
- 18+ years  

The dataset contains structured numerical values suitable for exploratory data analysis and statistical evaluation.

---

## 🛠️ Methodology
1. Data cleaning and validation  
2. Month-wise aggregation of enrollment data  
3. Pincode-wise aggregation  
4. Skewness detection  
5. Log transformation to handle extreme skewness  
6. Age-group contribution analysis  
7. Insight generation and interpretation  

---

## 📉 Skewness Analysis & Log Transformation

### Before Log Transformation
The data showed extreme right skewness due to a few pincodes having very high enrollment.

| Age Group| Skewness |
|----------|----------|
| 0–5      |       49 |
| 5–17     |       57 |
| 18+      |       29 |

### After Log Transformation
Log transformation significantly improved the data distribution.

| Age Group| Skewness |
|----------|----------|
| 0–5      |      1.0 |
| 5–17     |      1.7 |
| 18+      |      9.6 |

**Result:**  
Log transformation reduced the impact of outliers and made the data more suitable for comparison and visualization.

---

## 📆 Month-wise Enrollment Insights

### Age Group: 0–5 Years
- **Highest enrollment:** September (5000+ enrollments)
- **Lowest enrollment:** May (0–1000 enrollments)
- **Zero enrollment months:** February, March, April, August

### Age Group: 5–17 Years
- **Highest enrollment:** September (2000+ enrollments)
- **Lowest enrollment:** May (0–250 enrollments)
- **Zero enrollment months:** February, March, April, August

### Age Group: 18+ Years
- **Highest enrollment:** July (100+ enrollments)
- **Lowest enrollment:** December (0–20 enrollments)
- **Zero enrollment months:** February, March, April, August

**Insight:**  
Aadhaar enrollment is highly seasonal, with September emerging as the peak month, especially for children and students.

---

## 📊 Age Group Contribution

| Age Group | Contribution (%)|
|----------|------------------|
| 0–5      |     70.5%        |
| 5–17     |     28.1%        |
| 18+      |     1.4%         |

**Key Observation:**  
More than 98% of Aadhaar enrollments occur below 18 years, indicating that enrollment activity is predominantly child-centric.

---

## 📍 Pincode-wise Enrollment Analysis

### Highest Enrollment Pincode
- **423203**  
This pincode records the highest Aadhaar enrollment across all age groups.

### Lowest Enrollment Pincodes
| Age Group | Pincode |
|----------|--------- |
| 0–5      |   422209 |
| 5–17     |   422009 |
| 18+      |   422606 |

**Insight:**  
Low-enrollment pincodes may require improved accessibility, awareness campaigns, or mobile enrollment units.

---

## ✅ Conclusion
- Aadhaar enrollment in Nashik shows strong seasonal patterns
- September is the most critical enrollment month
- Children aged 0–5 years contribute the majority of enrollments
- Enrollment is highly concentrated in a few pincodes
- Adult enrollment (18+) is minimal and irregular

This analysis highlights the importance of **targeted and data-driven Aadhaar enrollment strategies**.

---

## 🔮 Future Work & Recommendations
- Analyze correlation with school admission cycles
- Perform year-over-year trend analysis
- Compare Nashik with other districts
- Identify high- and low-demand zones using clustering
- Deploy mobile enrollment units in low-performing pincodes
- Plan enrollment drives ahead of peak months

---

## 🚀 Tech Stack
- Python  
- Pandas  
- Matplotlib / Seaborn  
- Jupyter Notebook  
