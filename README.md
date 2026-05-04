# 🚗 Ride-Hailing Operations Analysis

An end-to-end Excel data analysis project exploring supply and demand 
patterns of a ride-hailing service across 35 days (Nov–Dec 2016).

## 📊 Project Overview

This project analyzes hourly operational data from a ride-hailing platform 
to uncover patterns in driver activity, ride fulfillment, and customer demand coverage.

## 📁 Dataset

| File | Description |
|------|-------------|
| Supply Data | Hourly driver activity — active drivers, online hours, finished rides |
| Demand Data | Hourly search overview — users served, unserved, coverage ratio |

- **Period:** November 14 – December 18, 2016
- **Records:** 839 hourly entries
- **Source:** Kaggle

## 🛠️ Tools Used

- Microsoft Excel (Power Query, XLOOKUP, PivotTables, Charts)

## ✅ Steps Performed

1. **Data Import** — Imported both CSV files into separate Excel sheets
2. **Data Cleaning** — Split Date & Hour columns, replaced nulls, removed duplicates, renamed columns, changed data types
3. **Data Merging** — Used XLOOKUP with a Key column (Date + Hour) to merge supply into demand data
4. **Feature Engineering** — Created new columns:
   - `Total_Demand` = Unserved + Served Users
   - `Total_Supply` = Finished Rides
   - `Supply_Demand_Gap` = Supply - Demand
   - `Fulfillment_Rate_%` = Served / Total Demand × 100
5. **Daily Summary** — Aggregated data by date using PivotTable
6. **Dashboard** — Built interactive dashboard with KPI cards and charts

## 📈 Dashboard Features

### KPI Cards
| Metric | Value |
|--------|-------|
| Total Finished Rides | 11,738 |
| Total Demand | 40,509 |
| Avg Coverage % | 75.7% |
| Avg Fulfillment % | 75.7% |

### Charts
- 📈 Daily Supply vs Demand trend
- 📊 Rides by Hour of Day
- 📈 Coverage % Trend Over Time
- 📈 Fulfillment Rate % Over Time

## 💡 Key Insights

- **Demand always exceeds supply** — a consistent gap exists throughout the period
- **Peak hours are 18:00–20:00** (evening rush) with highest ride volumes
- **December shows higher demand** than November, especially mid-December
- **Early morning hours (3–6 AM)** have lowest rides but high unserved users
- **Average coverage is 75.7%** meaning ~1 in 4 users couldn't find a car

## 📂 Workbook Structure

| Sheet | Contents |
|-------|----------|
| Dashboard | KPI cards + 4 charts |
| Analysis | Merged hourly data with all calculated columns |
| Supply | Cleaned supply raw data |
| Demand | Cleaned demand raw data |
| Daily_Summary | Day-wise aggregated data |

## 👤 Author

Made by [Jyothi Muddaboina]  
Connect on [Jyothi Muddaboina](https://www.linkedin.com/in/jyothi-muddaboina-86b699392/)
