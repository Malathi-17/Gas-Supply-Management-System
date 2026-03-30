Gas Inventory Management System

A desktop-based Gas Inventory Management System developed using Java (Swing GUI) in NetBeans with Oracle SQL as the backend database.
The system is designed to manage the complete workflow of gas order processing, including customer registration, order placement, verification, stock checking, delivery handling, payment recording, notifications, and feedback collection.

Project Overview

This application helps automate the operations of a gas distribution and inventory management process. It supports different stages of the supply workflow and provides a structured interface for handling customer orders and tracking stock availability.

The project was built as a database-driven desktop application and demonstrates the integration of Java frontend development with Oracle database operations using JDBC.

Features
Customer registration and data management
Order placement by customers
Order verification by retailer/employee
Stock availability checking
Delivery processing
Payment recording
Notification generation
Feedback collection
Oracle database integration
Swing-based desktop user interface
Technologies Used
Java
Java Swing
NetBeans IDE
Oracle SQL
JDBC
Modules Included
1. Customer Module

Allows customers to:

Register or enter details
Place gas orders
Select gas type and quantity
2. Order Verification Module

Allows retailer or employee to:

View placed orders
Verify or reject orders
Move verified orders to the next stage
3. Stock Checking Module

Used to:

Fetch verified orders
Check stock availability from the inventory
Confirm whether the requested quantity is available
4. Delivery Module

Used to:

Process confirmed deliveries
Update order status
Reduce stock after successful delivery
5. Payment Module

Used to:

Record payment details for completed deliveries
Store payment mode, amount, and related order details
6. Notification and Feedback Module

Used to:

Notify customers regarding order progress
Collect customer feedback after order completion
Database Tables Used

The project uses the following Oracle SQL tables:

Customer1
Retailer1
Manufacturer1
Orders1
Production
Stock
Distribution
Notification1
Delivery1
Payment1
Feedback
Workflow

The system follows this workflow:

Insert Order → Orders1
Verify Order → Retailer / Employee
Check Stock → Stock
Create Delivery → Delivery1
Update Inventory → Stock
Record Payment → Payment1
Notify Customer → Notification1
Collect Feedback → Feedback
How to Run the Project
Open the project in NetBeans IDE.
Make sure Oracle Database is running.
Import or create the required tables in your Oracle SQL environment.
Update your JDBC connection details in the Java files:
Host
Port
SID / Service Name
Username
Password
Add the Oracle JDBC driver (ojdbc) to your project libraries.
Run the main Java files step by step or through your dashboard.
Sample JDBC Connection
con = DriverManager.getConnection(
    "jdbc:oracle:thin:@localhost:1521:orcl",
    "scott",
    "tiger"
);
Learning Outcomes

This project demonstrates:

Java GUI development using Swing
Oracle database design and integration
JDBC connectivity
CRUD operations
Workflow-based desktop application design
Real-time stock and order management concepts
Future Enhancements

Possible improvements include:

Role-based login for customer, retailer, and manufacturer
Better dashboard navigation
Report generation
Search and filter functionality
Automated stock alerts
Improved UI design
Secure password handling

