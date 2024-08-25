Restaurant Management System Project Overview
1. Introduction
This project is a comprehensive restaurant management system designed to streamline the ordering process,manage tables, and handle payments.
The system integrates a graphical user interface (GUI) built using Python's Tkinter library with a MySQL database to store and manage order details.
The application allows restaurant staff to take orders, assign them to tables, process payments, and generate receipts.
Additionally, it features a tab where completed orders can be viewed, including details such as table numbers, payment methods, and items ordered.

2. Key Features
-Menu Management: The system allows the restaurant to maintain a dynamic menu.
Menu items can be added or removed as needed, and each item is categorized (e.g., Food, Drink, Dessert) with associated pricing.
-Order Management: Orders can be created by selecting items from the menu.
These orders can then be associated with specific tables in the restaurant.
-Table Management: The system manages multiple tables, allowing staff to assign orders to specific tables.
Tables can be marked as occupied when an order is assigned and cleared once the order is completed.
-Payment Processing: The system supports multiple payment methods (Cash, Credit Card, Digital Payment).
Upon processing the payment, the order status is updated, and the order details are saved to the database.
-Receipt Generation: After an order is paid for, the system generates a detailed receipt that includes the table number,
items ordered, total cost, and payment method.
-Completed Orders View: A dedicated tab displays all completed orders in a tabular format,
showing details like order ID, table number, total amount, payment method, and the items ordered.


3. Technical Components
-Graphical User Interface (GUI): The GUI is created using Tkinter,
which provides a user-friendly interface for restaurant staff to interact with the system.
The interface includes components like buttons, dropdown menus, and list boxes to facilitate easy navigation and operation.

-Database Integration: MySQL is used to store and manage order details.
The database schema includes tables for orders and order items,
with fields for storing essential information such as order ID, table number, total amount, payment method, and item details.
Object-Oriented Design: The project follows an object-oriented design, with classes such as MenuItem, Order, Table, Staff, Restaurant,
and Payment encapsulating different aspects of the restaurant’s operations. This modular design makes the system extensible and easy to maintain.

4. Classes and Their Responsibilities
-MenuItem: Represents a single item on the restaurant's menu. Each item has a name, price, and category.
-Order: Manages the items in a customer's order, calculates the total cost, handles payment processing,
and saves order details to the database. The order is associated with a specific table.
-Table: Represents a table in the restaurant. It tracks whether the table is occupied and the current order assigned to it.
-Staff: Represents a staff member in the restaurant (e.g., Waiter, Chef). Staff members can take orders and serve them.
-Restaurant: Manages the overall operations, including adding menu items, tables, and staff.
It also assigns orders to tables and handles the payment process.
-Payment: Manages the payment process for an order, handling different payment methods and updating the order status upon successful payment.
