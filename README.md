# 🍽️ Online Restaurant Menu Ordering System – DBMS Project

A robust and normalized **Database Management System (DBMS)** designed for smart restaurant operations—streamlining digital ordering, waiter-chef coordination, and billing—backed by optimized SQL queries and ER modeling.

---

## 📌 Problem Statement

Modern restaurants need digital transformation. This DBMS project solves:

- 🔸 Digital menu display at each table
- 🔸 Order placements linked to tables and customers
- 🔸 Real-time updates for kitchen & service staff
- 🔸 Automated billing with analytical reporting

It also logs edge cases like:
- 🚫 Order cancellations
- 🧾 Refunds
- 🚶 Walkouts (no-payment)

---

## 🧱 ER Diagram

> This ER Diagram visualizes the relationships among customers, waiters, chefs, menu items, and billing logic.

![ER Diagram](./assets/restaurant-er-diagram.png)

> Ensure the image is saved in `/assets/restaurant-er-diagram.png` or update the path as needed.

---

## 🗃️ Database Schema Overview

| Table Name         | Description |
|--------------------|-------------|
| `MENU`             | Dish ID, Name, Cost |
| `CD`               | Customer Details |
| `COD`              | Customer → Ordered Dishes |
| `WAITER_DETAILS`   | Waiter Info |
| `CHD`              | Chef Info |
| `CHOD`             | Chef → Dish Mappings |
| `OD`               | Order Metadata |
| `WOD`              | Waiter → Order → Chef Links |

---

## ⚙️ Features

### 🧾 CRUD Operations
- Add, update, and retrieve dishes, orders, waiters, chefs, customers.

### 🔄 Join Queries
- Real-time bill generation per table
- Chef-to-dish assignments
- Waiter-service logs

### 👁️ Views
- `ITEM_POPULARITY` – Most frequently ordered items
- `BILL_OF_ALL_CUSTOMERS` – Finalized bills across customers

### 📊 Reports & Insights
- Total restaurant revenue
- Dish-wise popularity
- Never-ordered dishes
- Chef-specific performance

### SQL Concepts Used:
- **JOINs**
- **Nested Queries**
- **Pattern Matching** (`LIKE`)
- **Aggregation** (`SUM`, `COUNT`, `AVG`)
- **Group By + Having**

---

## 💻 Technologies Used

- 🗃️ **Oracle SQL**
- 📈 **ER Diagram Modeling**
- 🛠️ **PL/SQL Procedures**
- 🧮 **3NF Normalization**
- 🚀 **Query Optimization**

---

## 🛠️ Setup Instructions

### 1. 📥 Clone the Repository

```bash
git clone https://github.com/prashantuppar618/restaurant-dbms.git
cd restaurant-dbms

