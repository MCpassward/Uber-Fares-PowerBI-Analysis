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


**Google colab python codes final result's Image after  cleanses **


<img width="1366" height="663" alt="4" src="https://github.com/user-attachments/assets/a030c265-e429-4d26-a29a-13c97932b997" />


**Power BI Reports Results Image**


![88](https://github.com/user-attachments/assets/8ec48067-c99c-4f84-acee-5d6608ec1128)

##For more :see all python codes and results in /`Images`/##

**Author:**  
Murenzi Charles  
INSY 8413 – Introduction to Big Data Analytics  
AUCA, July 2025

