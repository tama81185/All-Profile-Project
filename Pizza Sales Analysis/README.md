
# 🍕 Pizza Sales Analysis Project

## 📌 Project Overview
This project focuses on analyzing historical pizza sales data to uncover sales trends, customer ordering behavior, and product performance. The goal is to support restaurant management in making **data-driven decisions** related to pricing, promotions, inventory planning, and menu optimization.

---

## 🎯 Business Problem
The pizza restaurant lacks clear visibility into:
- Best-selling and underperforming pizzas
- Seasonal and time-based sales fluctuations
- Customer ordering patterns
- Revenue contribution by pizza category, size, and ingredients  

This makes it difficult to optimize the menu, manage inventory efficiently, and design effective promotions.

---

## ✅ Business Objectives
The objectives of this analysis are to:
- Identify **top-performing and low-performing pizzas**
- Measure **total revenue** and **average order value (AOV)**
- Discover sales trends by **date, day, and time**
- Analyze pizza popularity by **category and size**
- Provide actionable insights for **menu optimization and promotions**
- Enable management to make **data-driven decisions**

---

## 📂 Data Source
- **Dataset Name:** `pizza_sales.csv`

---

## 🧾 Data Description
| Column Name | Description |
|------------|-------------|
| order_id | Unique identifier for each customer order |
| pizza_id | Unique identifier for each pizza sold |
| pizza_name_id | System-defined pizza type and size code |
| pizza_name | Display name of the pizza |
| quantity | Number of pizzas sold per order |
| unit_price | Price per pizza |
| total_price | Total revenue per transaction |
| order_date | Date of order placement |
| order_time | Time of order placement |
| pizza_size | Pizza size (S, M, L, XL) |
| pizza_category | Pizza category (Classic, Veggie, Supreme, etc.) |
| pizza_ingredients | Ingredients used in the pizza |

---

## 📊 Key Performance Indicators (KPIs)
- **Total Revenue** = Sum of `total_price`
- **Total Pizzas Sold** = Sum of `quantity`
- **Total Orders** = Count of unique `order_id`
- **Average Order Value (AOV)** = Total Revenue ÷ Total Orders
- **Average Pizzas per Order** = Total Pizzas Sold ÷ Total Orders

---

## ❓ Business Questions Answered
- Which pizzas sell the **most and least** by quantity?
- What is the **monthly total revenue and average order value**?
- On which **days of the week** and **hours of the day** are orders highest?
- Which **pizza categories and sizes** are most popular?
- Are there **seasonal trends** affecting pizza sales?
- Which **ingredients** are most frequently used?
- Which pizza category generates the **highest total revenue**?
- How does **revenue vary by day**?
- Which pizzas generate the **most and least revenue**?
- What are the **top 10 most profitable pizzas**?
- What are the **peak ordering times** by:
  - Pizza category
  - Pizza size

---

## 🛠 Tools & Technologies
- **Python**
- **Pandas** – Data cleaning and analysis
- **NumPy** – Numerical operations
- **Matplotlib & Seaborn** – Data visualization
- **Jupyter Notebook** – Exploratory analysis

---

## 📈 Analysis & Visualizations
The project includes:
- Sales trends over time (daily, monthly)
- Revenue and order volume analysis
- Category-wise and size-wise performance
- Peak hour and weekday demand analysis
- Top and bottom-performing pizzas
- Ingredient usage insights

---

## 📌 Key Insights (Example)
- Certain pizza sizes and categories dominate total revenue
- Clear peak ordering times during lunch and dinner hours
- A small number of pizzas generate a large portion of total revenue
- Seasonal demand fluctuations suggest targeted promotions

---

## 🚀 Business Recommendations
- Focus promotions on **high-performing pizzas**
- Re-evaluate or redesign **low-performing menu items**
- Optimize inventory based on **peak hours and popular ingredients**
- Introduce time-based offers during **off-peak hours**
- Adjust pricing strategies using **AOV and profitability insights**

---

## 📁 Project Structure
