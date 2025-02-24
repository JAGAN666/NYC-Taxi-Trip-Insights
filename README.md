# NYC Taxi Trip Insights 🚖

## 📌 Project Overview
This project analyzes **NYC taxi trip records from 2012–2023** using **PySpark, Pandas, MLlib, and Sklearn** in **Google Colab**. The dataset, provided by the **NYC Taxi and Limousine Commission (TLC)**, captures billions of taxi rides, enabling insights into urban transportation patterns, fare predictions, and passenger behaviors.

---

## 📊 Key Insights from the Analysis

### 🔥 **1. Demand Hotspots & Taxi Utilization Patterns**
- **Peak Demand Locations:**
  - High demand is concentrated in **Manhattan** and **Brooklyn**, particularly in **business districts, airports, and tourist areas**.
  - **Times Square, Midtown, and Downtown Manhattan** emerge as the busiest pickup locations.

- **Time-Based Demand Trends:**
  - **Morning (7–10 AM) and evening (5–8 PM) rush hours** have the highest taxi demand.
  - **Late-night (11 PM–3 AM) rides surge** in entertainment zones.
  - Weekday demand follows a **commuter-driven pattern**, while weekends show increased night-time travel.

- **Heatmap Analysis:**
  - **Pickup density is highest** near major transit hubs like **Penn Station, Grand Central, JFK, and LaGuardia**.
  - Taxi availability is **lower in outer boroughs**, highlighting accessibility inefficiencies.

---

### 🤖 **2. Predictive Modeling & Machine Learning Applications**
#### 📍 **Trip Duration Prediction**
- **Key Findings:**
  - Strong correlation between **trip distance, pickup/drop-off location, and trip duration**.
  - Rush hour trips take **20–30% longer** than off-peak trips.

#### 💰 **Fare Estimation & Pricing Analysis**
- **Insights:**
  - **Fares are highest in Manhattan**, while **Brooklyn and Queens have lower fares**.
  - **Airport trips have fixed fares** (JFK: $52–$70, LaGuardia: varies).
  - The model accurately predicts **fare amounts based on borough, trip distance, and time of day**.

#### 🏷️ **Passenger Segmentation & Travel Behavior**
- **Three Passenger Clusters Identified:**
  1. **Short-Distance Travelers:** Prefer cash, frequent in **outer boroughs**.
  2. **Commuters & Business Travelers:** Use credit cards, active in **business hubs**.
  3. **Tourists & Late-Night Riders:** Higher fares, longer trips, common in **Manhattan & Airports**.

#### 💳 **Payment Type Prediction**
- **Cash vs. Card Usage Trends:**
  - **Cash payments are more common for short-distance rides** and in **outer boroughs**.
  - **Credit cards dominate Manhattan rides (75% of transactions).**

#### 🎁 **Tip Prediction & Customer Behavior**
- **Tip Amount Correlation:**
  - **Longer trips with higher fares receive better tips**.
  - **Rush hour delays slightly reduce tipping behavior**.

#### 💵 **High vs. Low Fare Classification**
- Early trip data helps in **predicting whether a trip will have a high or low fare**.

---

### 🚦 **3. Traffic Congestion Insights**
- **Traffic Bottlenecks Identified:**
  - **Congestion is worst in Lower Manhattan**, Midtown, and major bridges.
  - **Short trips in congested areas have longer durations due to traffic.**
  - **Weekend congestion is lower, but late-night traffic surges in entertainment zones.**

- **Congestion Prediction Model:**
  - **Historical trip data is used to forecast congestion hotspots**.

---

## 🔧 **Technical Approach & Methodology**
- **Data Processing:**
  - Handled **millions of records** using **PySpark** for high-performance computation.
  - Feature extraction: **trip duration, peak hours, fare structures, passenger behavior.**

- **Feature Engineering:**
  - Created **temporal features** (hour, day, weekend indicator).
  - Built **geographical clustering** for demand analysis.
  - Derived **tip percentage, fare breakdowns, and trip segmentation features**.

- **Machine Learning Models Used:**
  - **Regression:** Predict trip duration, fare, and tip amount.
  - **Classification:** Predict payment type (cash/card) and high vs. low fare.
  - **Clustering:** Passenger segmentation based on trip behavior.

- **Visualization & Reporting:**
  - Used **Matplotlib and Seaborn** to generate **heatmaps, bar charts, and time-series plots**.

---

## 🎯 **Business Impact & Use Cases**
✅ **Urban Transport Optimization**:
   - Identifies **high-demand areas** for optimized taxi fleet distribution.
   - Helps **develop peak pricing strategies**.

✅ **City Planning Benefits**:
   - Assists policymakers in **improving public transportation routes**.
   - Highlights underserved areas for **better taxi service availability**.

✅ **Customer Experience Improvements**:
   - **Fare prediction models** can provide passengers with **cost transparency**.
   - **Trip duration forecasting** improves **estimated wait times**.

---

## 📂 **Repository Structure**
