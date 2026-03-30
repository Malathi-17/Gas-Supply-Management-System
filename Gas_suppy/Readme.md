# 🔥 Gas Management System (Java + MySQL)

A desktop-based Gas Management System developed in **Java (NetBeans)** with backend integration using **MySQL**.  
The system manages cylinder bookings, customer details, billing, and inventory for a gas agency.

---

## 💡 Features

- 👥 Customer registration & management  
- 📦 Cylinder booking & tracking  
- 🧾 Automated billing system  
- 🛒 Inventory and stock monitoring  
- 🔐 Login authentication for staff/admin  
- 📊 Data stored in MySQL database

---

## 🛠️ Technologies Used

- **Java (Swing GUI)** – for frontend  
- **NetBeans IDE** – for development  
- **MySQL** – as backend database  
- **JDBC** – for Java-DB connectivity

---

## 🚀 How to Run

1. Open the project in **NetBeans** IDE.
2. Make sure **MySQL server is running**.
3. Import the SQL file (if any) to create the required database:
   - Use **phpMyAdmin** or any MySQL client.
   - Example:  
     ```sql
     CREATE DATABASE gas_management;
     USE gas_management;
     -- then create tables as required
     ```
4. Update the DB credentials in your Java code (usually in `DBConnection.java` or similar):
   ```java
   String url = "jdbc:mysql://localhost:3306/gas_management";
   String username = "root";
   String password = "your_password";
