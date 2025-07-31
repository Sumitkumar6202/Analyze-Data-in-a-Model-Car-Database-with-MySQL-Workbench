Model Car Database Analysis with MySQL Workbench
Overview
This project demonstrates how to analyze data in a model car database using MySQL Workbench. The database contains information about scale model cars, including products, customers, orders, and sales data. Through a series of SQL queries, we can extract valuable business insights from this dataset.

Database Schema
The database consists of the following tables:

Products: Model car details (product code, name, scale, vendor, quantity in stock, price)

ProductLines: Categories of model cars (classic, vintage, motorcycles, etc.)

Customers: Customer information and demographics

Orders: Sales transaction records

OrderDetails: Line items for each order

Employees: Sales representatives and their information

Offices: Regional office locations

https://schema-diagram.png (Note: Actual ER diagram would be shown here)

Setup Instructions
Prerequisites
MySQL Server (v8.0+ recommended)

MySQL Workbench

Sample database file (model_car_db.sql)

Installation Steps
Clone this repository:

bash
git clone https://github.com/yourusername/model-car-database-analysis.git
cd model-car-database-analysis
Create the database in MySQL:

sql
CREATE DATABASE model_car_db;
USE model_car_db;
Import the sample data:

Open MySQL Workbench

Go to Server → Data Import

Select "Import from Self-Contained File"

Choose model_car_db.sql

Start Import

Verify the installation:

sql
SHOW TABLES;
SELECT COUNT(*) FROM products;  -- Should return 110 records
