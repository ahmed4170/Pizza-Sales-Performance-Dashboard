# 🍕 Pizza Sales Performance Dashboard

## 📊 Project Overview
This project transforms raw transactional data from a pizza restaurant into a dynamic, interactive dashboard. By implementing a professional **Star Schema** data modeling approach, I analyzed over **48,600 orders** to uncover trends in customer behavior, peak sales periods, and product performance.

---

## 🛠️ Tech Stack
* **Tool:** Microsoft Excel
* **Data Engine:** Power Query (ETL) & Power Pivot (Data Modeling)
* **Analysis:** Pivot Tables & DAX (Data Analysis Expressions)
* **Visualization:** Interactive Excel Dashboard

---

## ⚙️ Project Workflow

### 1. Data Preprocessing (ETL)
Using **Power Query**, I cleaned and prepared the raw data for analysis:
* **Cleaning:** Removed duplicates, handled null values, and standardized naming conventions.
* **Date & Time Parsing:** Extracted years, months, and days from timestamps to enable time-series analysis.
* **Feature Engineering:** Created a custom `TimeSlot` column (Morning, Afternoon, Evening, Night) to identify peak operational hours.
* **Data Typing:** Formatted columns as Currency, Dates, and Whole Numbers to ensure calculation accuracy.

### 2. Data Modeling (Star Schema)
To optimize performance, I designed a **Star Schema** in Power Pivot. This involved separating the data into a central Fact table and several Dimension tables:
* **Fact Table (`FactSales`):** Stores all transactional data, including quantities and total prices.
* **Dimension Tables:** * `DimPizza`: Product names and ingredients.
    * `DimCategory`: High-level categories (Classic, Veggie, Supreme, Chicken).
    * `DimSize`: Pizza size variations (S, M, L, XL, XXL).
    * `DimDate`: Calendar hierarchy for monthly and quarterly trends.
    * `DimTime`: Time-based attributes including the engineered `TimeSlot`.
* **Relationships:** Established 1-to-Many relationships using unique keys to ensure seamless data filtering.

### 3. Data Analysis
I performed deep-dive analysis using **Pivot Tables** and **DAX** to calculate core business metrics:
* **Total Revenue:** $817,860.05
* **Total Pizzas Sold:** 49,574
* **Total Orders:** 48,620
* **Average Order Value:** $16.82
* **Performance Ranking:** Identified top-selling products by revenue and quantity.

### 4. Dashboard Designing
The final stage was the creation of a user-centric, interactive interface:
* **Visual Selection:** Used Bar Charts for product rankings, Donut Charts for category distribution, and Area/Line Charts for sales trends.
* **Interactivity:** Integrated **Slicers** (Category, Size, Date) and **Timelines** to allow users to filter the entire report with one click.
* **UI/UX:** Organized a logical flow where high-level KPIs are at the top, followed by detailed breakdowns of time and product performance.

---

## 🔍 Key Insights
* **Revenue Leader:** The **Classic** category is the primary revenue driver ($220K+), while the **Thai Chicken Pizza** is the individual top performer ($43.4K).
* **Peak Demand:** The **Afternoon** (12 PM – 4 PM) and **Evening** (4 PM – 8 PM) slots account for the vast majority of sales, generating over $700,000 combined.
* **Size Preference:** **Large (L)** size pizzas are the most popular, contributing significantly more to revenue ($375.3K) than Medium or Small sizes.

---

## 🖼️ Dashboard Preview
![Dashboard Main View](images/dashboard_main.png)
*(Upload your dashboard screenshot to an 'images' folder and link it here)*

## 📐 Data Model View
![Data Model View](images/data_model.png)
*(Upload a screenshot of your Power Pivot Diagram View here)*

---

## 🚀 How to Use
1. Download the `Final Project.xlsx` file from this repository.
2. Open the file in Microsoft Excel.
3. Click "Enable Content" if prompted to allow Data Connections and Power Pivot.
4. Interact with the **Slicers** and **Timeline** on the Dashboard sheet to explore the data.

---
**Contact:** [Your Name] | [Your LinkedIn Profile]
