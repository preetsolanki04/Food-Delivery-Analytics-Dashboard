# 🍔 Food Delivery Dashboard – Power BI Project

## 📌 Project Overview

The **Food Delivery Dashboard** is an end-to-end **Power BI analytics project** designed to analyze food delivery operations, customer behavior, restaurant performance, and delivery efficiency.

This project demonstrates **data cleaning, data modeling, DAX calculations, and interactive dashboard creation** to generate meaningful business insights for a food delivery platform.

---

# 🛠 Tools & Technologies

* **Power BI Desktop**
* **Power Query Editor**
* **DAX (Data Analysis Expressions)**
* **Data Modeling**
* **Interactive Dashboard Design**

---

# 📂 Project Workflow

## 1️⃣ Import Dataset

* Imported raw dataset into **Power BI Desktop**
* Verified file structure and column formats.

---

## 2️⃣ Inspect Columns

* Checked column names
* Verified data types
* Identified missing values
* Identified duplicate records.

---

## 3️⃣ Data Cleaning & Transformation (Power Query)

Performed the following steps in **Power Query Editor**:

* Removed duplicates
* Handled missing values
* Standardized column names
* Converted data types
* Trimmed text values
* Removed unnecessary columns

---

## 4️⃣ Create `RestaurantID`

Generated a **unique identifier for restaurants** to support data modeling and relationships.

Example:

```
RestaurantID = R001, R002, R003 ...
```

---

# 🗂 Data Modeling

## 5️⃣ Finalize Restaurants Table

Contains restaurant related information:

* RestaurantID
* Restaurant Name
* City
* Cuisine Type
* Rating

---

## 6️⃣ Create Orders Table

Contains order transaction details:

* OrderID
* RestaurantID
* CustomerID
* Order Amount
* Order Status
* Delivery Time
* Order Date

---

## 7️⃣ Create Customers Table

Contains customer information:

* CustomerID
* Customer Name
* Location
* Order Count
* Total Spend

---

## 8️⃣ Create Date Table

Created a **Date dimension table** for time-based analysis.

Example columns:

* Date
* Day
* Month
* Quarter
* Year
* Weekday

Example DAX:

```
DateTable = CALENDAR(MIN(Orders[OrderDate]), MAX(Orders[OrderDate]))
```

---

## 9️⃣ Build Relationships

Created relationships between tables:

| Table  | Column       | Relationship |
| ------ | ------------ | ------------ |
| Orders | RestaurantID | Restaurants  |
| Orders | CustomerID   | Customers    |
| Orders | Date         | DateTable    |

Model Type: **Star Schema**

---

# 🧮 DAX Calculations

## 🔹 Calculated Columns

Created calculated columns for:

* Delivery Duration
* Order Category
* Customer Segments

---




---

# 📊 Dashboard Pages

## 📍 Page 1 — Overview

High level business metrics:

* Total Orders
* Total Revenue
* Total Customers
* Average Order Value
* Revenue Trend
* Orders by City

---

## 👥 Page 2 — Customer Analysis

Customer behavior insights:

* Top Customers
* Customer Spending
* Orders per Customer
* Customer Distribution by Location

---

## 🍽 Page 3 — Restaurant Performance

Restaurant performance tracking:

* Top Performing Restaurants
* Revenue by Restaurant
* Restaurant Ratings
* Orders by Cuisine Type

---

## 🚚 Page 4 — Delivery & Operations

Operational performance metrics:

* Average Delivery Time
* Delivery Success Rate
* Orders by Status
* Delivery Trends

---

## 📈 Page 5 — Advanced Insights

Deep analytical insights:

* Peak Order Hours
* Revenue Trends
* Seasonal Demand
* Customer Segmentation

---

## 🏪 Page 6 — Restaurant Details

Detailed restaurant analysis:

* Restaurant specific KPIs
* Order trends
* Revenue contribution
* Customer ratings

---

# 🎛 Interactive Features

## 🔹 Slicers

Added slicers for:

* Date
* City
* Restaurant
* Cuisine
* Order Status

---

## 🔹 Visual Interactions

Configured **cross filtering and cross highlighting** between visuals for better exploration.

---

# 🎨 Final Formatting

Final dashboard improvements:

* Consistent color theme
* Clear KPI cards
* Proper visual alignment
* Dynamic titles
* User-friendly layout

---

# 📊 Key Business Insights

This dashboard helps stakeholders to:

✔ Monitor platform performance
✔ Identify top restaurants
✔ Understand customer behavior
✔ Improve delivery efficiency
✔ Track revenue growth

---

# 🚀 Future Improvements

* Real-time data integration
* Predictive analytics for demand forecasting
* Customer churn prediction
* Delivery route optimization

---

# 📁 Project Structure

```
Food-Delivery-Dashboard
│
├── dataset
│   └── food_delivery_data.csv
│
├── dashboard
│   └── Food_Delivery_Dashboard.pbix
│
└── README.md
```

---

# 👨‍💻 Author

**Preet Solanki**

Data Analyst | Power BI | SQL | Python

---

⭐ If you like this project, consider giving it a **star on GitHub!**
