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

**Power BI File:**
**🔗 [Here  ](https://drive.google.com/file/d/1NFrtK7DaJ8u16HRmnni6OP-gqzFprx6I/view)**

**Tools Used:**
- Python (Pandas, NumPy, Matplotlib)
- Power BI Desktop
- GitHub (for documentation and final delivery)

**Workflow:**
1. Imported the raw dataset using Python and Pandas.
```
import pandas as pd

# Load the dataset
df = pd.read_csv("uber.csv")
df.head()
```
🔍Inspect Data
```
# See info about columns
df.info()

# Check for missing values
df.isnull().sum()
```
2. Performed Exploratory Data Analysis (EDA) to examine structure and quality.
3. 🧹Cleaned the dataset:
   - Removed nulls and duplicates.
   - Filtered out invalid fare amounts and distances.
```
# Drop 'Unnamed: 0' column
df.drop(columns=['Unnamed: 0'], inplace=True)

# Convert pickup_datetime to datetime
df['pickup_datetime'] = pd.to_datetime(df['pickup_datetime'], errors='coerce')

# Drop rows with missing values
df.dropna(inplace=True)

# Remove negative or zero fare amounts
df = df[df['fare_amount'] > 0]

# Filter passenger count to a valid range (1 to 6)
df = df[(df['passenger_count'] >= 1) & (df['passenger_count'] <= 6)]
```

**<img width="1365" height="660" alt="1" src="https://github.com/user-attachments/assets/7a7504ce-60cc-4329-a7c5-3358f848e468" />
<img width="1366" height="701" alt="2" src="https://github.com/user-attachments/assets/571b6c2a-e067-433d-ad6c-ec876dacf8bf" />
<img width="1366" height="700" alt="3" src="https://github.com/user-attachments/assets/ffa18d41-83a4-4314-ae57-ea7cf5c53056" />**
4. Engineered new features:
   - Extracted `hour`, `day`, `month`, and `year` from timestamp.
   - Created peak/off-peak indicators and weekday categories.
5. 💾Saved the cleaned dataset as a `.csv` file for Power BI import.
```
# Save cleaned data for Power BI
df.to_csv("uber_cleaned.csv", index=False)
```
**<img width="1366" height="663" alt="4" src="https://github.com/user-attachments/assets/a030c265-e429-4d26-a29a-13c97932b997" />**
6. Import into Power BI and built the dashboard.

---

## 📊 Analysis: Detailed Findings and Statistical Insights

**Descriptive Statistics:**
- **Mean fare:** \$11.35  
- **Median fare:** \$8.50  
- **Max fare:** \$497.00  
- **Common fare range:** \$7–\$15  
- **Peak ride hours:** 5 PM – 8 PM
```
# Descriptive statistics
mean_fare = df['fare_amount'].mean()
median_fare = df['fare_amount'].median()
mode_fare = df['fare_amount'].mode()[0]
std_fare = df['fare_amount'].std()

# Quartiles
quartiles = df['fare_amount'].quantile([0.25, 0.5, 0.75])
data_range = df['fare_amount'].max() - df['fare_amount'].min()

# Display results
print(f"Mean Fare: {mean_fare:.2f}")
print(f"Median Fare: {median_fare:.2f}")
print(f"Mode Fare: {mode_fare:.2f}")
print(f"Standard Deviation: {std_fare:.2f}")
print(f"Quartiles:\n{quartiles}")
print(f"Range: {data_range:.2f}")
```
**<img width="1032" height="487" alt="99" src="https://github.com/user-attachments/assets/d75c98cd-1365-4e36-838b-3c53b5a5f750" />**

**Visual Insights:**
- **Fare Patterns by Hour**: Sharp increases during morning and evening peaks.
- **Hourly Ride Patterns**: Majority of rides happen in the afternoon and evening.
- **Monthly Patterns**: Summer and holiday seasons (July, December) have more rides.
- **Seasonal Trends**: Yearly increase in ride activity in Q3 and Q4.
- **Ride Duration (by Drop-off Year)**: Highest in 2014–2015.
- **Location Pickup Map**: Dense ride clusters in New York, San Francisco, and other major cities.

**Variable Relationships:**
- Strong correlation between **fare amount** and **trip distance**.
  **<img width="1356" height="665" alt="6" src="https://github.com/user-attachments/assets/c5ec8e3e-6433-4e8c-9c3d-eb464a7b9293" />**
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

## Screenshots ##


**Google colab python codes for cleanses**





<img width="1360" height="702" alt="5" src="https://github.com/user-attachments/assets/5a50b721-a8fa-4692-b2e4-b308a3977059" />

<img width="1366" height="658" alt="7" src="https://github.com/user-attachments/assets/e620cb3a-2695-424a-a076-35d4d00bad61" />
<img width="1366" height="660" alt="8" src="https://github.com/user-attachments/assets/9a6dbbd0-8ff0-4292-bfa8-766749e53fde" />



**Power BI Reports Results Image**


![88](https://github.com/user-attachments/assets/8ec48067-c99c-4f84-acee-5d6608ec1128)



**For more :see all screenshots of python codes and results in /`Images`/**

**Author:** 

Murenzi Charles

**Instructor:**

Lec.Maniraguha Eric

Course – Introduction to Big Data Analytics  
AUCA, July 2025

