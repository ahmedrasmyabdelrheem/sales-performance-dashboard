# Sales & Revenue Performance Executive Dashboard

## 📌 Project Overview
An executive sales analytics dashboard engineered entirely in **Microsoft Excel** using **Power Pivot** and **DAX**. 

The project consolidates historical transactional data into a relational data model (Star Schema) to analyze over **$3.5M in revenue** across 1,000 orders. It evaluates sales performance across regional territories, customer segments, delivery timelines, and seasonal spikes.

---

## 🎯 Business Problem & Objectives
- **Data Fragmentation:** Sales and operational data were stored in siloed sheets without relational integrity.
- **Limited Analytics:** Standard Pivot Tables could not handle multi-table calculations or complex time-based metrics without heavy formula overhead.
- **Objective:** Construct a centralized dimensional data model in Power Pivot and author advanced DAX measures to deliver executive insights on order fulfillment and profit margins.

---

## 🏗️ Technical Architecture & Modeling

```text
[Raw Excel Tables]
  - Orders, Customers, Products, and Locations
         ↓
[Power Pivot Data Model]
  - Star Schema architecture (Fact_Orders linked to Dimensions)
  - 1-to-Many relationships with defined cross-filter direction
         ↓
[Advanced DAX Layer]
  - Custom KPI measures using iterator functions (SUMX, AVERAGEX)
  - Delivery cycle duration calculations (DATEDIFF)
         ↓
[Executive Reporting Layer]
  - Interactive Excel dashboard with linked slicers and KPI cards
