# WFoods_Retail_Management_system

# 🛒 WFOODS Retail Data Analytics Project

## 📊 Project Overview
This project represents a complete end-to-end data analytics workflow using retail data from WFOODS. It simulates real-world business scenarios by transforming raw CSV files into meaningful insights through data cleaning, modeling, analysis, and visualization.

The project demonstrates how data analysts convert raw data into actionable business intelligence for decision-making.

---

## 🎯 Objective
- Clean and transform raw CSV datasets  
- Build a scalable data model  
- Perform advanced analysis using DAX  
- Create interactive dashboards in Power BI  
- Generate business insights and recommendations  

---

## 🛠️ Tools & Technologies
- **Power BI** (Power Query, Data Modeling, DAX, Visualization)  
- **SQL** (Data querying & validation)  
- **Excel / CSV Files** (Data source)  

---

## 🔄 Project Workflow

### 1️⃣ Data Cleaning & Transformation (Power Query)

#### 📌 Customers Table
- Promoted headers and renamed table  
- Corrected data types  
- Created:
  - `full_name` (first + last name)  
  - `birth_year` from birthdate  
  - `has_children` (Y/N based on total_children)  

---

#### 📌 Products Table
- Fixed data types  
- Created `discount_price` (90% of retail price)  
- Rounded to 2 decimal places  
- Analyzed:
  - 111 unique brands  
  - 1,560 product names  
- Replaced null values with 0  
- Calculated average retail price by brand  

---

#### 📌 Stores Table
- Created:
  - `full_address` (city, state, country)  
  - `area_code` from phone number  

---

#### 📌 Regions Table
- Validated structure and data types  

---

#### 📌 Calendar Table
Generated time intelligence columns:
- Start of Week  
- Day Name  
- Month Name  
- Quarter  
- Year  

---

#### 📌 Transactions Data
- Combined 1997 & 1998 datasets  
- Cleaned and validated data  
- Ensured proper date range  

---

#### 📌 Return Data
- Validated data types and structure  

---

### 2️⃣ Data Modeling

- Built a **Star Schema** with:
  - Fact Tables: Transactions, Returns  
  - Dimension Tables: Customers, Products, Stores, Calendar, Regions  

- Established relationships:
  - One-to-many cardinality  
  - Single direction filters  
  - Snowflake schema (Stores → Regions)  

- Optimized model:
  - Hidden foreign keys  
  - Applied proper formatting and categorization  

---

### 3️⃣ Data Analysis using DAX

#### 📌 Calculated Columns
- Weekend flag  
- End of Month  
- Customer Age  
- Customer Priority  
- Price Tier (Low / Mid / High)  
- Years Since Remodel  

---

#### 📌 Key Measures
- Quantity Sold: **833,489**  
- Quantity Returned: **8,289**  
- Total Transactions: **269,720**  
- Total Revenue: **$1,764,546**  
- Total Cost: **$711,728**  
- Total Profit: **$1,052,819**  
- Profit Margin: **59.67%**  
- Return Rate: **0.99%**  

---

#### 📌 Advanced Metrics
- Weekend Transactions (28.4%)  
- YTD Revenue  
- 60-Day Rolling Revenue  
- Last Month Performance Metrics  
- Revenue Target (5% growth logic)  

---

### 4️⃣ Data Visualization (Power BI Dashboard)

#### 📊 Topline Performance Dashboard Includes:
- KPI Cards (Transactions, Profit, Returns)  
- Matrix (Top 30 Brands Performance)  
- Map (Transactions by City)  
- Treemap (Country → State → City drilldown)  
- Weekly Revenue Trend Chart  
- Revenue vs Target Gauge  

---

### 📌 Interactive Features
- Drill-down & drill-up functionality  
- Slicers (Country filter)  
- Bookmarks for insights storytelling  
- Navigation buttons  
- Role-Level Security (RLS) for country managers  

---

### 5️⃣ Key Insights
- High-performing product brands drive majority revenue  
- Weekend transactions contribute significantly (~28%)  
- Certain cities (e.g., Portland) show strong sales spikes  
- Profit margins are high (~60%), indicating strong pricing strategy  
- Low return rate (~1%) reflects customer satisfaction  

---

### 💡 Business Recommendations
- Focus marketing on top-performing brands  
- Increase inventory in high-demand regions  
- Optimize pricing for mid-tier products  
- Target weekend promotions for higher sales  
- Use regional insights for localized strategies  

---


