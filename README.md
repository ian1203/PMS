# PMS
# Product Management System

This is a **Java-based Product Management System** that allows users to manage products in a database. The system provides a **Graphical User Interface (GUI)** for adding, updating, deleting, and viewing products. It uses **Java Swing** for the frontend and **PostgreSQL** for the backend database.

---

## Features

1. **Add Product**:
   - Add a new product with details such as ID, name, code, category, quantity, purchase price, retail price, and supplier.

2. **Update Product**:
   - Modify the details of an existing product.

3. **Delete Product**:
   - Remove a product from the database using its code.

4. **View Products**:
   - Display all products in a table with columns for ID, name, code, category, quantity, purchase price, retail price, and supplier.

5. **Database Integration**:
   - The system connects to a PostgreSQL database to store and retrieve product data.

---

## Technologies Used

- **Java**: Core programming language.
- **Java Swing**: For building the graphical user interface.
- **PostgreSQL**: Database for storing product information.
- **JDBC**: Java Database Connectivity for interacting with the database.

---

## Prerequisites

Before running the project, ensure you have the following installed:

1. **Java Development Kit (JDK)**: Version 8 or higher.
2. **PostgreSQL**: Installed and running on your machine.
3. **IDE**: IntelliJ IDEA, Eclipse, or any Java-supported IDE.
4. **PostgreSQL JDBC Driver**: Required for connecting Java to PostgreSQL.

---

## Setup Instructions

### 1. Database Setup

1. **Create a Database**:
   - Open PostgreSQL and create a new database named `pms`.
   ```sql
   CREATE DATABASE pms;
   CREATE TABLE products (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    code INT NOT NULL,
    category VARCHAR(50),
    quantity INT NOT NULL,
    purchase_price DECIMAL(10, 2) NOT NULL,
    retail_price DECIMAL(10, 2) NOT NULL,
    supplier VARCHAR(100)
);

private static final String URL = "jdbc:postgresql://localhost:5433/pms";
private static final String USER = "your_username";
private static final String PASSWORD = "your_password";

git clone https://github.com/your-username/product-management-system.git
