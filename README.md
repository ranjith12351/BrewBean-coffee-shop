# ☕ BrewBean Coffee Shop — Business & Sales Analytics Project

---

## 📌 Executive Summary & Project Overview

BrewBean Coffee Shop is a high-growth multi-outlet coffee retail brand operating across 9 regional store locations (Gandhipuram, RS Puram, Peelamedu, Saravanampatti, Pollachi, Trichy, Salem, Tiruppur, and Madurai). 

This project delivers an end-to-end Data Analytics solution designed to evaluate store sales performance, revenue drivers, customer buying patterns, hourly peak-load bottlenecks, and promotional campaign efficacy. By processing raw transactional logs through Python, Power Query, and Excel, this analysis transforms complex operational data into actionable business strategies for executive decision-makers.

---

## 📊 Executive KPI & Financial Performance Baseline

| Core Metric Category | Measured Baseline Value | Target Benchmark | Variance Analysis & Strategic Assessment |
| :--- | :---: | :---: | :--- |
| **Gross Revenue** | **$293,688.48** | $300,000.00 | 🟢 **97.8% Target Realization:** Strong top-line performance driven by urban flagship stores. |
| **Net Earnings (Profit)** | **$175,869.48** | $170,000.00 | 🟢 **+3.45% Outperformance:** Excellent bottom-line growth reflecting strong cost control. |
| **Gross Profit Margin** | **65.2%** | 60.0% | 🟢 **Robust Unit Economics:** High profit retention across core hot & cold beverage categories. |
| **Total Order Volume** | **800 Orders** | 1,000 Orders | 🟡 **Capacity Gap:** Foot traffic density restricted by morning counter bottlenecks. |
| **Units Moved** | **44,572 Units** | 50,000 Units | 🟡 **Healthy Velocity:** High basket-size throughput during peak operating hours. |
| **Average Order Value (AOV)** | **$367.11** | $300.00 | 🟢 **High Basket Value:** Strong cross-category sales between drinks and bakery products. |
| **Customer Satisfaction (CSAT)** | ⚠️ **3.4 / 5.0** | **4.5 / 5.0** | 🔴 **CRITICAL BOTTLENECK:** Customer drop-off caused by morning rush hour queue delays. |

---

## 🎯 Key Strategic Insights & Business Findings

### 1. Revenue Concentration & Regional Footprint Disparity
* **Urban Hub Dominance:** Top 3 outlets—**Gandhipuram, RS Puram, and Peelamedu**—generate over **52% of total multi-store revenue** ($35,000+ per store), functioning as primary profit drivers.
* **Tier-2 Expansion Vulnerability:** Outlets in **Salem, Tiruppur, and Madurai** experience lower revenue density despite identical pricing and cost structures.
* **Margin Uniformity:** Profit margins remain static at **~65% across all 9 stores**, confirming that regional underperformance is purely driven by **store foot-traffic volume**, not product cost inefficiencies.

### 2. Operational Rush Hour Dynamics & Capacity Bottlenecks
* **Morning Peak Surge (08:00 AM – 09:00 AM):** Accounts for the single largest hourly transaction spike of the day. Driven by daily commuters and office professionals, this peak directly correlates with long queue delays and lower CSAT scores (3.4 / 5.0).
* **Evening Leisure Surge (05:00 PM – 07:00 PM):** Secondary surge window focused heavily on high-margin cold chillers and bakery snacks.
* **Mid-Day Labor Inefficiency (11:00 AM – 01:00 PM):** Significant reduction in transaction density resulting in underutilized store staff and high idle labor overhead.

### 3. Payment Gateway Ecosystem & Checkout Velocity
* **Digital Market Dominance (>85%):** **GPay / Google Pay** leads payment processing at **40%**, followed closely by **PhonePe / UPI** at **29%**.
* **Cash & Card Processing Delays:** Cash transactions (**16%**) and Credit/Debit card processing (**13%**) create significant counter delay during rush hours due to manual terminal handling.

### 4. Product Packaging & Inventory Real-Estate Efficiency
* **Core Beverage Engine (Cups):** Hand-crafted beverages sold in **Cups** represent **over 23,000+ units**, proving that fresh hot and cold coffees remain the primary brand anchor.
* **Packaged Retail Stagnation (Bottles & Packs):** Pre-packaged retail coffee items show the lowest inventory turnover rate, unproductively locking up display shelf real estate.

---

## 🛠️ Data Analytics Workflow & Tools Used

The analysis was executed using a dedicated Data Analytics toolkit:

```text
[ Raw Transactional Data ] 
       │
       ▼
┌────────────────────────────────────────────────────────────────────────┐
│ 1. DATA CLEANING & PREPROCESSING (Python - Pandas & NumPy)             │
│    • Ingestion of raw Excel/CSV dataset                                │
│    • Duplicate removal, missing value imputation, & data type casting  │
│    • Categorical standardization (Payment methods, item categories)    │
└────────────────────────────────────────────────────────────────────────┘
       │
       ▼
┌────────────────────────────────────────────────────────────────────────┐
│ 2. DATA TRANSFORMATION & SHAPING (Power Query)                         │
│    • Merging transaction tables with store metadata & product catalogs │
│    • Creating custom conditional columns & hourly time-bucket groups   │
│    • Power Query M-code transformations for clean data aggregation     │
└────────────────────────────────────────────────────────────────────────┘
       │
       ▼
┌────────────────────────────────────────────────────────────────────────┐
│ 3. DATA ANALYSIS & VISUAL DASHBOARD (Microsoft Excel)                  │
│    • Advanced Pivot Tables & Pivot Charts for dynamic aggregation      │
│    • Excel formulas (XLOOKUP, SUMIFS, AVERAGEIFS, INDEX/MATCH)         │
│    • Interactive Slicers, Timeline filters, & Executive Dashboard      │
└────────────────────────────────────────────────────────────────────────┘
