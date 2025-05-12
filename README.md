🗃️ Inventory Management System (SQL Project)
📄 Description
This SQL-based Inventory Management System helps manage product stock levels, categorize items, track suppliers, and monitor sales activity. It's a simple yet functional schema ideal for understanding basic database design and operations such as table relationships, inserting data, and performing queries.

The project includes:

Supplier management

Category classification

Product tracking

Sales tracking and inventory updates

It’s great for learning how foreign keys, default values, and data integrity work in MySQL.

⚙️ How to Set Up / Run the Project
Install MySQL
Make sure you have MySQL or a MySQL-compatible tool (e.g., MySQL Workbench, phpMyAdmin, or XAMPP) installed on your system.

Create and Use the Database
Run the following commands to create and select your working database:

sql
Copy
Edit
CREATE DATABASE inventory_db;
USE inventory_db;
Create Tables
Execute the SQL commands to create the following tables:

Suppliers

Categories

Products

Sales

Insert Sample Data
Insert initial records into each table to test your setup.

Run Queries
Example query to view product stock levels along with their supplier and category:

sql
Copy
Edit
SELECT 
  p.product_name, 
  p.quantity_in_stock, 
  p.price, 
  c.category_name, 
  s.supplier_name
FROM 
  Products p
JOIN Categories c ON p.category_id = c.category_id
JOIN Suppliers s ON p.supplier_id = s.supplier_id;
