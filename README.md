# 🏥 Hospital Management System - Java GUI Project

This is a **Java-based Hospital Management System** developed using **Swing (GUI)** and **MySQL** for database operations. The project was built as the **final project for my first university term**, and it offers a comprehensive interface for managing hospital data such as patients, employees, rooms, departments, and ambulances.

---

## Features

-  **Login System** with authentication
-  **Add New Patients**
-  **Update Patient Details**
-  **View All Patients Info**
-  **Room Management** (Availability, Price, Type)
-  **Ambulance Info Display**
-  **Department Info Display**
-  **Employee Info Display**
-  **Patient Discharge System**
-  **Search Rooms by Availability**
-  **Logout Functionality**

---

##  User Interface

- Built with **Java Swing** for a responsive and easy-to-use GUI.
- Icons and buttons are used to provide a modern user experience.
- Main dashboard (Reception) acts as the central hub for navigation.

---

##  Tech Stack

- **Language:** Java (JDK 20)
- **GUI Framework:** Swing
- **Database:** MySQL
- **IDE:** IntelliJ IDEA
- **External Libraries:**
    - `mysql-connector-java-8.0.28.jar`
    - `rs2xml.jar` (for displaying `ResultSet` in `JTable`)

---

##  Project Structure

- All source code is in the package: `hospital.management.system`
- Main classes include:
    - `Login`
    - `Reception`
    - `NEW_PATIENT`
    - `update_patient_details`
    - `ALL_Patient_Info`
    - `Employee_info`
    - `Room`
    - `Ambulance`
    - `Department`
    - `patient_discharge`
    - `SearchRoom`
    - `conn` (handles DB connection)

---

##  How to Run

1. **Clone the Repository**  
   git clone https://github.com/your-username/hospital-management-system.git
   cd hospital-management-system

markdown
Copy
Edit

2. **Set Up Database**
- Use MySQL and run the SQL script provided (`hospital_db.sql`) to create the required database and tables.
- Make sure MySQL is running.

3. **Configure Database Connection**  
   In `conn.java`, make sure to set your local MySQL credentials:
```java
connection = DriverManager.getConnection(
    "jdbc:mysql://localhost:3306/hospital_management_systems", 
    "your_mysql_username", 
    "your_mysql_password"
);
Add Dependencies

Add the following JAR files to your project structure in IntelliJ:

mysql-connector-java-8.0.28.jar

rs2xml.jar

Run the Program
Run Login.java to start the application.

🗂️ Database Schema
Tables Created:
login

patient_info

room

department

ambulance

emp_info

Sample Data Inserted:
sql
Copy
Edit
INSERT INTO login (ID, PW) VALUES ('hospitalmanagement', '12345');

INSERT INTO Room VALUES ("100", "Available", "500", "G Bed 1");
-- More rooms...

INSERT INTO department VALUES ("Surgical department", "051-8653345");
-- More departments...

INSERT INTO Ambulance VALUES ("AMB-001", "Basic Life Support", "Available", "0300-1234567");
-- More ambulances...

INSERT INTO EMP_INFO VALUES ("Doctor 1", "38", "03376538653", "158,000", "dr@gmail.com", "23");
-- More employees...

![Project Structure Screenshot](![img.png](src/icon/img.png)icon/img.png)

The following dependencies were added to the project:

✅ mysql-connector-java-8.0.28.jar

✅ rs2xml.jar


📚 Educational Purpose
This project was created as part of my first-term final project at university. It helped me understand how to:

Build interactive desktop applications with Java Swing

Establish database connections with JDBC

Structure real-world applications using object-oriented programming

Use MySQL for data persistence and operations

📌 Note
This project is for educational purposes only and may not be suitable for production use without further enhancements and security updates.

📬 Contact
For feedback or collaboration, feel free to reach out via GitHub or email.

🏁 License
This project is licensed under the MIT License.