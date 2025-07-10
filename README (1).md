
# 🛒 Inventory Management System

A simple **console-based inventory management system** built using **Java (NetBeans IDE)** and **MySQL**, designed for managing product stock in a small retail store.

---

## ✅ Features

- ➕ Add new products to the inventory
- 🔁 Update existing product quantities
- ❌ Remove products from the inventory
- 📋 View all products in a clean format

---

## 🧰 Tech Stack

| Technology | Description |
|------------|-------------|
| Java       | Backend logic (NetBeans IDE 8.2) |
| MySQL      | Relational database (using SQLyog) |
| JDBC       | Java Database Connectivity |

---

## 🗂️ Project Structure

```
InventoryManagementSystem/
├── AddProduct.java
├── UpdateProduct.java
├── RemoveProduct.java
├── ViewProducts.java
├── DBConnection.java
└── InventoryManagementSystem.java (Main file)
```

---

## 🛠️ How to Run

### 🧾 Step 1: MySQL Setup

1. Open SQLyog or your preferred MySQL client
2. Run the following SQL:

```sql
CREATE DATABASE IF NOT EXISTS inventory_db;

USE inventory_db;

CREATE TABLE IF NOT EXISTS products (
    id INT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    quantity INT NOT NULL
);
```

---

### 🧑‍💻 Step 2: Run in NetBeans

1. Open the project in **NetBeans 8.2**
2. Ensure **MySQL JDBC connector** is added to project libraries
3. Open `InventoryManagementSystem.java` file
4. Run the file

You will see the following menu in the console:

```
1. Add Product
2. Update Product Quantity
3. Remove Product
4. View All Products
5. Exit
```

---

## 📌 Notes

- Database name: `inventory_db`
- Table name: `products`
- DB username/password: Update in `DBConnection.java` if needed

```java
con = DriverManager.getConnection("jdbc:mysql://localhost:3306/inventory_db", "root", "root");
```

---

## 👨‍💻 Developed By

**Hardik Bakhatriya**  
Email: [your email]  
Phone: [your number]

---

## 📎 License

This project is for educational/demo purposes only.
