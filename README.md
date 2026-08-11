# 🍕 Pizza Sales SQL Project

A SQL-based data analysis project on pizza sales data — covering revenue trends, best-selling pizzas, order patterns, and category-wise performance using **joins, aggregations, subqueries, and window functions**.

## 📌 Project Overview

This project analyzes a pizza restaurant's sales dataset to answer business questions like which pizzas sell the most, which categories generate the highest revenue, and how orders are distributed throughout the day. The goal was to practice real-world SQL querying — from basic aggregations to advanced window functions.

## 🗂️ Database Schema

The database consists of 4 related tables: `pizza_types`, `pizzas`, `orders`, and `order_details`.



<img width="1280" height="555" alt="pizza_sales_schema png" src="https://github.com/user-attachments/assets/af76da0b-3b6f-48d1-928f-d04d358a27e1" />



- **pizza_types** — pizza name, category, ingredients
- **pizzas** — size and price variants for each pizza type
- **orders** — order date and time
- **order_details** — links orders to pizzas with quantity ordered

## 🛠️ Tools Used

- SQL (MySQL)
- Dataset: Pizza Sales dataset

## ❓ Business Questions Solved


1. Retrieve the total number of orders placed
2. Calculate the total revenue generated from pizza sales
3. Identify the highest-priced pizza
4. Identify the most common pizza size ordered
5. List the top 5 most ordered pizza types along with their quantities


6. Find the total quantity of each pizza category ordered
7. Determine the distribution of orders by hour of the day
8. Find the average number of pizzas ordered per day
9. Determine the top 3 pizza types based on revenue



10. Calculate the percentage contribution of each pizza category to total revenue
11. Analyze the cumulative revenue generated over time
12. Determine the top 3 pizza types based on revenue for each pizza category

## 📁 Files in this Repository

| File | Description |
|---|---|
| `schema.sql` | Table creation scripts (database structure) |
| `queries.sql` | All 12 analysis queries with explanations |
| `pizza_sales_schema.png` | Entity-relationship diagram of the database |

## 📊 Key Results

| Metric | Value |
|---|---|
| Total Orders Placed | 21,350 |
| Total Revenue Generated | ₹8,17,860.05 |
| Highest-Priced Pizza | The Greek Pizza (₹35.95) |
| Most Common Pizza Size | Large (18,526 orders) |
| Average Pizzas Ordered per Day | 138 |

**Top 5 Most Ordered Pizza Types**
| Pizza | Quantity |
|---|---|
| The Classic Deluxe Pizza | 2,453 |
| The Barbecue Chicken Pizza | 2,432 |
| The Hawaiian Pizza | 2,422 |
| The Pepperoni Pizza | 2,418 |
| The Thai Chicken Pizza | 2,371 |

**Top 3 Pizza Types by Revenue**
| Pizza | Revenue |
|---|---|
| The Thai Chicken Pizza | ₹43,434.25 |
| The Barbecue Chicken Pizza | ₹42,768.00 |
| The California Chicken Pizza | ₹41,409.50 |

**Revenue Contribution by Category**
| Category | Revenue Share |
|---|---|
| Classic | 26.91% |
| Supreme | 25.46% |
| Chicken | 23.96% |
| Veggie | 23.68% |

**Order Quantity by Category**
| Category | Quantity |
|---|---|
| Classic | 14,888 |
| Supreme | 11,987 |
| Veggie | 11,649 |
| Chicken | 11,050 |

**Pizza Size Distribution**
| Size | Orders |
|---|---|
| Large | 18,526 |
| Medium | 15,385 |
| Small | 14,137 |
| XL | 544 |
| XXL | 28 |

## 💡 Key Insights

- Peak ordering hours are **12 PM–1 PM** and **6 PM–7 PM**, aligning with lunch and dinner rushes
- **Large** is the most preferred pizza size, followed closely by Medium and Small
- The **Classic** category generates the highest revenue share (~27%), despite Chicken pizzas dominating individual top-sellers by revenue
- Revenue and order patterns were tracked over time using window functions (`SUM() OVER`)
- Category-wise and pizza-wise ranking was done using `RANK() OVER (PARTITION BY ...)`

## 🚀 How to Run

1. Create the database using `schema.sql`
2. Import the pizza sales dataset into the respective tables
3. Run any query from `queries.sql` to get the corresponding insight

---

⭐ If you found this project useful, feel free to star the repo!
## 👤 Author

**Preet**
