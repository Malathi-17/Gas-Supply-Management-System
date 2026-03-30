##Gas Inventory Management System

A desktop-based Gas Inventory Management System developed using Java (Swing GUI) in NetBeans with Oracle SQL as the backend database. The system is designed to manage the complete workflow of gas order processing, including customer order placement, order verification, stock checking, delivery handling, and payment recording.

##Project Overview

This application automates the operations of a gas distribution and inventory management process. It provides a structured workflow for handling gas orders, monitoring stock, updating inventory, and managing customer-related transactions through a Java-based desktop interface connected to an Oracle database using JDBC.

The project demonstrates the integration of frontend development in Java Swing with backend database operations in Oracle SQL.

##Features
Customer order placement
Order verification by retailer or employee
Stock availability checking
Delivery processing
Inventory update after delivery
Payment recording
Oracle database integration
Swing-based desktop user interface
Technologies Used
Java
Java Swing
NetBeans IDE
Oracle SQL
JDBC
##Modules
1. Customer Module

This module allows the customer to:

Enter customer details
Select gas type
Enter quantity
Place an order
2. Order Verification Module

This module allows the retailer or employee to:

View pending orders
Verify or reject customer orders
Move verified orders to the next step
3. Stock Checking Module

This module is used to:

Fetch verified orders
Match order details with available stock
Check whether sufficient stock is available
4. Delivery Module

This module is used to:

Confirm delivery details
Update order status to "Delivered"
Reduce stock quantity after successful delivery
5. Payment Module

This module is used to:

Record payment details
Store payment amount and mode
Maintain payment records for completed orders
Database Tables Used

##The project uses the following Oracle SQL tables:

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
Workflow

##The system follows this process:

Customer places an order and data is inserted into Orders1.
Retailer or employee verifies the order.
Verified orders are checked against available stock in the Stock table.
If stock is sufficient, delivery is processed.
After delivery, stock is updated by reducing the delivered quantity.
Payment details are recorded in the Payment1 table.
How to Run the Project
Open the project in NetBeans IDE.
Make sure Oracle Database is running.
Create the required tables in Oracle SQL.
Add the Oracle JDBC driver to your NetBeans project libraries.
Update the database connection credentials in your Java files.
Run the project from the main Java file.
Sample Database Connection

##Use a JDBC connection similar to the following in your Java files:

Connection con = DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:orcl", "scott", "tiger");

##Important Note

Ensure that your Oracle table column names exactly match the column names used in your Java SQL queries. If any column was created using double quotes, such as "Quantity", then the same exact case-sensitive name must be used in your SQL statements.

##Learning Outcomes

This project demonstrates:

Java Swing GUI development
Oracle SQL integration
JDBC connectivity
CRUD operations
Inventory and order workflow implementation
Real-time database interaction through desktop applications
Future Enhancements

##Possible improvements for this project include:

Role-based login for customer, retailer, and manufacturer
Notification system for order status updates
Feedback collection module
Search and filter functionality
Better UI design and dashboard navigation
Secure password handling
##Author
Malathi,Krithik Sai,Prawin
##Conclusion

The Gas Inventory Management System provides a structured and database-driven solution for managing gas orders and stock operations. It simplifies the workflow of order placement, verification, stock checking, delivery, and payment through a desktop application built using Java and Oracle SQL.
