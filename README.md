# Uber-Fares-PowerBI-Analysis
# 🚖 Uber Fares Dataset Analysis Report

## 📘 Introduction: Project Overview and Objectives

This project analyzes the Uber Fares dataset obtained from Kaggle to uncover insights related to fare patterns, ride behavior over time, and spatial trends. The primary goal is to use Power BI to create an interactive dashboard that supports data-driven decision-making for Uber’s operational strategies.

**Objectives:**
- Understand fare and ride patterns over time and space.
- Identify key periods and regions with high demand.
- Provide business insights through data storytelling and visualization.

---

## 🧪 Methodology: Data Collection and Analysis Approach

**Data Source:**  
Uber Fares Dataset from [Kaggle](https://www.kaggle.com)

**Tools Used:**
- Python (Pandas, NumPy, Matplotlib)
- Power BI Desktop
- GitHub (for documentation and final delivery)

**Workflow:**
1. Imported the raw dataset using Python and Pandas.
2. Performed Exploratory Data Analysis (EDA) to examine structure and quality.
3. Cleaned the dataset:
   - Removed nulls and duplicates.
   - Filtered out invalid fare amounts and distances.
4. Engineered new features:
   - Extracted `hour`, `day`, `month`, and `year` from timestamp.
   - Created peak/off-peak indicators and weekday categories.
5. Saved the cleaned dataset as a `.csv` file for Power BI import.
6. Imported into Power BI and built the dashboard.

---

## 📊 Analysis: Detailed Findings and Statistical Insights

**Descriptive Statistics:**
- **Mean fare:** \$11.35  
- **Median fare:** \$8.50  
- **Max fare:** \$497.00  
- **Common fare range:** \$7–\$15  
- **Peak ride hours:** 5 PM – 8 PM

**Visual Insights:**
- **Fare Patterns by Hour**: Sharp increases during morning and evening peaks.
- **Hourly Ride Patterns**: Majority of rides happen in the afternoon and evening.
- **Monthly Patterns**: Summer and holiday seasons (July, December) have more rides.
- **Seasonal Trends**: Yearly increase in ride activity in Q3 and Q4.
- **Ride Duration (by Drop-off Year)**: Highest in 2014–2015.
- **Location Pickup Map**: Dense ride clusters in New York, San Francisco, and other major cities.

**Variable Relationships:**
- Strong correlation between **fare amount** and **trip distance**.
- Fare values increase during **peak hours** and **weekends**.

---

## 🧩 Results: Key Discoveries and Pattern Identification

- Evening hours and weekends show the highest demand and fare values.
- Ride volumes peak in **July** and **December**, confirming seasonal patterns.
- Geographic hotspots are concentrated in urban areas like NYC and California.
- The fare distribution is positively skewed, with many mid-range fares and a few high-value outliers.

---

## ✅ Conclusion: Summary of Main Findings

Uber ride and fare patterns are significantly influenced by:
- **Time of day**
- **Day of the week**
- **Seasonality**
- **Geographic location**

These patterns provide clear evidence that Uber's demand and pricing strategy are aligned with user behavior, but also show opportunities for optimization.

---

## 📌 Recommendations: Data-Driven Business Suggestions

1. **Increase Driver Availability** during peak hours and high-demand seasons.
2. **Enhance Dynamic Pricing** around holidays and evening time slots.
3. **Expand into Underserved Areas** identified in spatial heatmaps.
4. **Create Promotions** for off-peak hours to encourage usage.
5. **Align Marketing Campaigns** with peak seasonal windows (summer and year-end).

---

## 📎 Appendix

**Dashboard Highlights:**
- Fare distribution charts
- Hourly and monthly ride visualizations
- Ride duration pie chart
- Geographic pickup locations map

## All screenshots of Results ##


#Google colab python codes results Image #


<img width="1365" height="660" alt="1" src="https://github.com/user-attachments/assets/d0677e68-c0a9-4fc4-bc95-2cb20016a501" />
<img width="1366" height="701" alt="2" src="https://github.com/user-attachments/assets/b61f93ec-912e-436e-bb75-fbf96585b720" />
<img width="1366" height="700" alt="3" src="https://github.com/user-attachments/assets/ae687d21-053e-4370-8ce1-1ac3f6e49926" />
<img width="1366" height="663" alt="4" src="https://github.com/user-attachments/assets/d947660a-4d55-412a-bf34-03fd46d92f5c" />
<img width="1360" height="702" alt="5" src="https://github.com/user-attachments/assets/86f2ea91-299c-45e4-bd2e-3e46ae301ddd" />
<img width="1356" height="665" alt="6" src="https://github.com/user-attachments/assets/67d8a0bd-0517-426e-af00-9d2145203c60" />
<img width="1366" height="658" alt="7" src="https://github.com/user-attachments/assets/e357330e-406f-41c7-bdf7-f69a152125f7" />
<img width="1366" height="660" alt="8" src="https://github.com/user-attachments/assets/7a4dae11-0626-49db-8956-faea8e620ec6" />


#POWER bi Reports Results Image#


![88](https://github.com/user-attachments/assets/8ec48067-c99c-4f84-acee-5d6608ec1128)


**Author:**  
Murenzi Charles  
INSY 8413 – Introduction to Big Data Analytics  
AUCA, July 2025

