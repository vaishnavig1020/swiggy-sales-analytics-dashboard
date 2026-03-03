# 🚀 Swiggy Sales & User Analytics Dashboard

An end-to-end Business Intelligence project built using Power BI to analyze sales performance, customer behavior, and city-level revenue trends.

---

## 📌 Problem Statement

Swiggy’s business data contains valuable insights across:
- Revenue trends
- Customer demographics
- Restaurant performance
- City-wise contribution

However, raw data alone does not reveal:
- Revenue concentration risk
- High-value customer segments
- Growth slowdowns
- Regional performance gaps

A structured analytical dashboard was required to convert raw data into actionable business insights.

---

## 💡 Solution

Developed an interactive Power BI dashboard that:

- Tracks Total Revenue & Order Trends
- Identifies Top 10% revenue-contributing customers
- Analyzes user demographics (Age, Marital Status, Occupation)
- Compares Veg vs Non-Veg performance
- Evaluates Restaurant-level revenue dominance
- Measures City-wise Revenue & ARPU

The dashboard is divided into:
1. Overview
2. User Performance
3. City Performance
4. Business Insights

---

## 📊 Key Insights

- 💰 **Total Revenue:** 964M
- 👥 Top 10% customers contribute ~75% of total revenue
- 📉 Orders peaked in 2018 (61K) followed by a slowdown
- 🥗 Veg category drives higher volume
- 🍗 Non-Veg category delivers 27% higher average price (better margins)
- 👤 Age 22–26 accounts for 60%+ users
- 💍 Single users generate 2x revenue compared to married users
- 🏙 Tirupati leads revenue (~43M)
- 💳 ARPU: 12.42K

---

## 📈 Business Impact

This dashboard enables decision-makers to:

- Design loyalty programs for high-value customers
- Address revenue concentration risk
- Identify underperforming cities
- Optimize pricing & promotional strategies
- Improve monetization using ARPU insights

---

## 🛠 Tools & Technologies

- Power BI
- DAX (Data Analysis Expressions)
- Data Modeling
- KPI Design
- Business Intelligence

---

## 🧮 Important DAX Measures

```DAX
Revenue LY = CALCULATE([Total Revenue], SAMEPERIODLASTYEAR(Date[Date]))

Revenue YoY % = 
DIVIDE([Total Revenue] - [Revenue LY], [Revenue LY])

ARPU = DIVIDE([Total Revenue], [Total Users])
