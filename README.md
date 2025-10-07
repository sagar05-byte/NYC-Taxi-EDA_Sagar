# 🚕 Exploratory Data Analysis: Optimising NYC Taxi Operations

### 📘 Assignment ID: EDA/02  
**Total Marks:** 200  
**Author:** Sagar Fadtare  
**Topic:** NYC Yellow Taxi Trip Data Analysis  
**Goal:** Optimise taxi operations, improve revenue, and identify efficiency patterns using data-driven insights.

---

## 📊 1. Project Overview
This project performs an **Exploratory Data Analysis (EDA)** on NYC taxi trip data to understand travel patterns, fare structures, demand trends, and operational efficiency.  
The outcome is a set of **actionable insights and recommendations** to optimise taxi utilisation and pricing strategies.

---

## 🧾 2. Dataset Description

| File | Description |
|------|--------------|
| `yellow_tripdata_YYYY-MM.parquet` | Monthly trip data containing pickup/dropoff, fare, and trip details |
| `taxi_zones.shp` | NYC taxi zone shapefile used for geographical visualisation |
| `cleaned_data.csv` | Processed dataset after cleaning and transformation |
| `plots/` | Folder containing all generated visualisations (PNG format) |

---

## 🧹 3. Data Cleaning Summary
Performed using Python (Pandas, NumPy):
- Removed duplicates and handled missing values  
- Fixed negative or invalid monetary amounts  
- Combined airport fees and added new derived fields:
  - `trip_duration`
  - `trip_speed`
  - `fare_per_mile`
- Removed outliers for `fare_amount`, `trip_distance`, and `payment_type=0`

---

## 📈 4. Exploratory Data Analysis

### 4.1 Temporal Analysis
- Trips by hour, day, and month
- Identified **rush hours (8–10 AM, 6–8 PM)**  
- **Weekdays** show higher average trips vs **weekends**

🖼️ *Figures:*  
`plots/hourly_trips.png`, `plots/daily_trends.png`

---

### 4.2 Financial Analysis
- Fare distribution and correlation with distance
- Tip percentage by vendor and passenger count
- Identified zones with **high average fare per mile**

🖼️ *Figures:*  
`plots/fare_distribution.png`, `plots/tips_by_payment.png`

---

### 4.3 Geographical Analysis
- Heatmaps of pickup/dropoff locations
- Mapped busiest taxi zones (e.g., Manhattan core)
- Zone-wise trip density visualised using shapefile overlays

🖼️ *Figures:*  
`plots/pickup_heatmap.png`, `plots/zone_density_map.png`

---

### 4.4 Passenger and Operational Insights
- Passenger count distribution (most trips = 1 or 2 passengers)
- Average speed vs distance trends
- Idle time and low-efficiency trip patterns detected

🖼️ *Figures:*  
`plots/passenger_distribution.png`, `plots/speed_vs_distance.png`

---

## 💡 5. Key Insights
- Demand peaks during **morning and evening rush hours**  
- **Downtown Manhattan** contributes the highest trip count  
- **Short trips** generate higher fare per mile than long trips  
- **Tips** are higher for credit card payments  
- **Low passenger count** trips dominate (1–2 passengers)

---

## 🚀 6. Recommendations
1. **Fleet Allocation:** Concentrate taxis in Manhattan during peak hours.  
2. **Dynamic Pricing:** Increase fares during demand spikes.  
3. **Route Optimisation:** Encourage shared rides in low-demand areas.  
4. **Operational Efficiency:** Track idle times and improve driver utilisation.  
5. **Customer Incentives:** Offer discounts on non-peak hours to balance demand.

---

## 🧠 7. Tools & Technologies
- **Python:** Pandas, NumPy, Matplotlib, Seaborn, Geopandas  
- **Data Format:** Parquet, Shapefile, CSV  
- **Environment:** Jupyter Notebook  

---

## 🧩 8. Outcomes
This analysis helps optimise NYC taxi operations by:
- Enhancing revenue through data-driven pricing  
- Improving trip efficiency and route planning  
- Understanding passenger and payment behaviour  
- Providing a foundation for predictive demand modelling  

---

## 📂 Folder Structure
NYC_Taxi_EDA_Assignment/
│
├── notebook.ipynb
├── cleaned_data.csv
├── plots/
│ ├── hourly_trips.png
│ ├── fare_distribution.png
│ ├── pickup_heatmap.png
│ └── tips_by_payment.png
└── README.md


---

## ✉️ Contact
**Author:** Sagar Fadtare  
For any clarification, please contact via GitHub or LinkedIn.m
