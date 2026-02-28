# 🏭 Production Monitoring Dashboard

> ⚡ This dashboard uses DAX measures to dynamically calculate **Efficiency %**, **Rejection %**, and **Production Variance** based on user-selected filters.

---

## 📌 Project Overview

The **Production Monitoring Dashboard** is an interactive Power BI solution designed to monitor and analyze manufacturing performance.

It compares planned vs actual production, tracks rejection rates, measures operational efficiency, and identifies machine-level performance issues to support data-driven decision-making in a production environment.

The dataset was cleaned and prepared using Microsoft Excel before being modeled and visualized in Power BI.

---

## 🎯 Business Objectives

- Monitor daily production output
- Compare Planned vs Actual production performance
- Track machine-wise rejection percentage
- Measure overall production efficiency
- Identify machines requiring attention
- Support operational performance improvement

---

## 🛠️ Tools & Technologies Used

- Microsoft Excel (Data Cleaning & Preparation)
- Power BI (Data Modeling & Visualization)
- DAX (Data Analysis Expressions)

---

## 📂 Project Structure

### 📊 Dashboard File

dashboard/Production_Monitoring_Dashboard.pbix

This Power BI file contains:

- Interactive KPI Cards
- Planned vs Actual Production Trend
- Machine-wise Production Analysis
- Rejection % Tracking
- Efficiency % Monitoring
- Performance Status Indicator

Open this file using **Power BI Desktop** to explore full interactivity.

---

### 📁 Dataset File

data/cleaned_production_data.xlsx

### Data Preparation Performed in Excel:

- Removed duplicate records
- Handled missing values
- Standardized date formats
- Structured dataset for reporting
- Prepared data for Power BI modeling

This dataset serves as the primary data source for the dashboard.

---

## 🧮 DAX Measures Implemented

The following DAX measures were created for dynamic KPI calculations:

- Efficiency %
- Rejection %
- Variance %
- Production Variance

### Example DAX Logic:

```DAX
Efficiency % = DIVIDE([Good Qty], [Actual Qty])

Rejection % = DIVIDE([Rejection Qty], [Actual Qty])

Variance % = DIVIDE([Actual Qty] - [Planned Qty], [Planned Qty])
