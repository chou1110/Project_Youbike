# YouBike Risk Analysis Project

## Overview
This project aims to identify potential **safety risks** at YouBike stations across Taipei City. By analyzing accident data and bike ridership records, this study provides **decision support** for improving bike station safety and urban planning.

## Objectives
- 🚲 **Identify high-risk YouBike stations** based on accident data and ridership statistics.
- ⚠ **Evaluate fatality risks** across Taipei City.
- 📊 **Provide actionable insights** for safety improvements.

## Methodology

### 1️⃣ Data Sources
- **Traffic accident records** (A1 & A2 accident data, 2021 latest)
- **YouBike 2.0 rental records** (latest 12 months)
- **YouBike 1.0 rental records** (latest 12 months)
- **YouBike station information & real-time data**

### 2️⃣ Risk Calculation Model
Risk is defined as:
```
Risk = Exposure × Hazard
```
Two different algorithms are used for risk evaluation:

#### **Algorithm 1: Single-Station Risk**
- Each station's risk is calculated based on the number of accidents within a defined **risk radius (r)**.
- Risk Score = Number of rides × Number of accidents at that station.
- Results tend to **highlight city center stations** with high ridership.

#### **Algorithm 2: Multi-Station Risk**
- Accidents are weighted by their **proximity to multiple stations**.
- Stations closer to accidents contribute more to the overall risk score.
- Results show a **more distributed risk pattern across the city**.

## Results
- 🔝 **Top 50 highest-risk stations identified**.
- 🟠 **Top 10 high-risk stations highlighted in orange**.
- 📍 **金華杭州南路口(2.0) ranks #1 in both algorithms**.
- 🚦 **Algorithm 1 results:** High-risk stations are mostly in the **city center**.
- 🌐 **Algorithm 2 results:** Risk is **more evenly spread** across the city.
- 🔄 **Additional insights:**
  - ~10% of trips **start and end at the same station**.
  - **Evening peak usage is higher and lasts longer** than the morning peak.

## Outputs
- **[Algorithm 1 Results](output/m1.html)** 🔗
- **[Algorithm 2 Results](output/m2.html)** 🔗