# 🍕 Pizza Sales & Operations Analytics Dashboard

## 📌 Executive Summary
An end-to-end Data Analytics and Business Intelligence project leveraging **Excel**, **Power Query**, and **Power BI** to analyze 48,000+ pizza sales records. 

The project delivers an interactive 2-page Executive Dashboard providing operational insights on peak sales hours and simulating dynamic pricing strategies to maximize revenue.

---

## 🏗️ Project Architecture & Workflow
1. **Data Ingestion & Cleaning (Power Query / ETL):**
   * Processed raw transactional data (48k+ rows).
   * Handled regional date formats (`Locale` standardizations) and resolved null/type mismatches.
   * Standardized data types for numerical metrics and time attributes.

2. **Feature Engineering:**
   * Extracted `Hour` and `Day Name` from transaction timestamps.
   * Created custom categorical logic (`Peak Bucket`) to classify operations into: `Lunch Peak`, `Afternoon Slow`, `Dinner Peak`, and `Late Night / Off-Peak`.

3. **Data Modeling & DAX Calculations:**
   * Designed a dedicated `_Measures` table for organized metric governance.
   * Calculated core business metrics: `Total Revenue`, `Total Orders`, `AOV` (Average Order Value), and `Total Pizzas Sold`.
   * Developed advanced scenario analysis measures using **What-If Parameters** to simulate dynamic price adjustments during peak hours.

---

## 📊 Dashboard Overview & Key Features

### 📄 Page 1: Operations Overview
* **KPI Metrics Bar:** Instant visibility on overall revenue ($818K), total orders (21K), and AOV ($38).
* **Peak Hours Heatmap (Matrix Visual):** Conditional formatting highlighting high-volume order slots by day and hour.
* **Hourly Category Breakdown:** Ribbon/Line chart depicting hourly demand across pizza categories (`Chicken`, `Classic`, `Supreme`, `Veggie`).

### 📄 Page 2: Dynamic Pricing & Scenario Simulation
* **Interactive What-If Parameter:** Allows decision-makers to adjust price multipliers during peak buckets (-10% to +20%).
* **Revenue Lift Analysis:** Dynamic DAX calculations tracking expected revenue increase and percentage growth.
* **Comparative Visuals:** Clustered bar charts comparing baseline revenue vs. simulated dynamic revenue by operational time bucket.

---

## 📈 Key Business Insights
* **Peak Demand Windows:** Highest order concentration occurs during **Lunch Peak (12 PM - 2 PM)** and **Dinner Peak (6 PM - 8 PM)**.
* **Dynamic Pricing Potential:** Applying a modest **+5% to +14% surge pricing** during peak hours yields an additional **$115K+ in revenue (~14.10% lift)** without significantly impacting order volume.

---

## 🛠️ Tools & Technologies Used
* **Power BI Desktop:** Data Modeling, DAX, Visual Design, What-If Parameters.
* **Power Query (M Engine):** ETL, Data Cleansing, Custom Conditional Columns.
* **Microsoft Excel:** Initial Data Auditing & Pivot Table Heatmaps.

---

## 📁 Repository Structure

├── data/
│   └── pizza_sales.csv
├── dashboard/
│   └── Pizza_Sales_Dashboard.pbix
├── screenshots/
│   ├── Operations_Overview.png
│   └── Dynamic_Pricing_Simulation.png
└── README.md

----

## 🛡️ License

This project is licensed under the MIT License. You are free to use, modify, and share this project with proper attribution.

## 🌟 About Me

Hi there! I'm Ahmed Alnaggar. I'm a data analyst.
