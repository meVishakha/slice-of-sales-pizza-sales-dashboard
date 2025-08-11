🍕 Slice of Sales - Pizza Sales Dashboard

📌 Project Overview
The Slice of Sales dashboard is a Power BI report designed to analyze pizza sales data and uncover key business insights.  
It provides interactive visuals to track sales performance, order trends, bestsellers, and product categories.

This project demonstrates **data visualization, DAX calculations, and storytelling with data** to make informed business decisions.

---

📂 Dataset
The dashboard is based on a fictional **Pizza Sales Dataset** containing:
- Pizza name, category, size
- Ingredients list
- Unit price, total price, and quantity sold
- Order date & time

---

📊 Key Features
- **Orders by Time**: Identifies peak ordering hours.
- **Pizza Category Analysis**: Classifies pizzas into Classic, Supreme, Veggie, and Chicken.
- **Sales by Size**: Shows distribution of orders across different pizza sizes (S, M, L, XL, XXL).
- **Top 10 Bestsellers**: Highlights the most popular pizzas by sales.
- **KPIs**:
  - Total Pizzas Made
  - Total Sales
  - Most Expensive Pizza
  - Cheapest Pizza
  - Number of Pizza Types

---

🧮 DAX Measures Used
```DAX
Total Sales = SUM('Pizza sales dataset'[total_price])

Most Expensive Pizza = MAX('Pizza sales dataset'[unit_price])

Cheapest Pizza = MIN('Pizza sales dataset'[unit_price])

Total Quantity = SUM('Pizza sales dataset'[quantity])

Types of Pizzas = DISTINCTCOUNT('Pizza sales dataset'[pizza_name])
