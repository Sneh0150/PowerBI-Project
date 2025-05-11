# 🧸 Reveue Analysis of Toy Shop

## 📌 Project Objective

This project focuses on analyzing Revenu data from a toy shop to generate actionable insights. It involves cleaning messy data, normalizing it into a star schema, creating an effective data model, and building an interactive dashboard in Power BI.

---

## Tools & Technologies Used

- **Power BI**
- **Power Query**
- **DAX (Data Analysis Expressions)**

---

## Project Workflow

### 🔹 1. Data Cleaning

- Raw data contained **blank rows**, **blank columns**, and was in an **unstructured format**.
- Utilized **Power Query Editor** to:
  - Remove nulls and irrelevant columns.
  - Rename columns and ensure consistent formatting.
  - Set correct data types.

---

### 🔹 2. Data Normalization

- Transformed the flat-file structure into a **star schema** for optimized data modeling.
- Created the following tables:

#### Fact Table:
- `Fact_Sales`: Includes sales metrics like Revenue, Quantity, Profit, along with keys for Date, Store, and Product.

#### Dimension Tables:
- `Dim_Store`: Store attributes such as Name, Type, Region.
- `Dim_Region`: Region names and hierarchy.
- `Dim_Date`: A calendar table for time-based analysis.
---

### 🔹 3. Data Modeling

- Established **relationships**:
  - `Fact_Sales` ➝ `Dim_Store`
  - `Fact_Sales` ➝ `Dim_Region`
  - `Fact_Sales` ➝ `Dim_Date`

- Used **one-to-many** relationships and ensured referential integrity.!
- ![Snip_dataModel](https://github.com/user-attachments/assets/63d45c3b-1b31-409b-9622-a1735b4efd8e)


### 🔹 4. KPI Metrics Implemented

- **Total Revenue vs Previous Month**
- **Total Quantity vs Previous Month**
- **Total Profit vs Previous Month**

Implemented using **DAX measures** such as `PREVIOUSMONTH()`, `CALCULATE()`, and `DATEADD()` for time intelligence.

---

### 🔹 5. Key Visuals & Insights

- **Revenue Trend by Weekdays** 
- **Store Type Revenue Share** 
- **Top Performing Product** vs Others
- **Top Performing Store** 

## 🚧 Challenges

- Creating a **dynamic calculation** to display:
  - Top N Product and group others as "Others"
  - Top N Store.
---
![Project ToyReveue](https://github.com/user-attachments/assets/0ef85d2f-b8c0-4720-833e-553a972e4818)


## ✅ Final Outcome

- Delivered an interactive and business-focused **Power BI dashboard**.
- Enabled month-over-month comparison of sales KPIs.
- Identified key revenue drivers and top-performing entities.
- Facilitated data-driven decisions for store and product strategies.

---




