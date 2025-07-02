# 🏥 Hospital Management System

This is a **Java GUI-based Hospital Management System** created as part of my **first-year programming project at NUST**. It provides basic hospital operations management such as patient registration, room allocation, employee info, ambulance tracking, and department listings — all through a simple, intuitive interface built using **Java Swing** and **MySQL**.

---

##  Features

###  Login System
- Secure login functionality for staff using MySQL-based credentials.

###  Patient Management
- Add new patient with ID, disease, room assignment, and deposit.
- View all patients with details.
- Update patient details like room, deposit, admission time.
- Discharge patients (automatically updates room availability).

###  Room Management
- View all hospital rooms with current availability and pricing.
- Search rooms by availability (Available / Occupied).
- Auto-update room status upon patient admission/discharge.

###  Ambulance Module
- View ambulance ID, type (Basic/Advanced Life Support), availability, and contact number.

###  Employee Information
- View all employees including name, age, phone, salary, Gmail, and ID.

###  Department Listing
- Access list of hospital departments and their phone numbers.

---

## 🛠 Tech Stack

| Layer       | Technology                                |
|-------------|--------------------------------------------|
| Language    | Java                                       |
| GUI         | Java Swing                                 |
| Database    | MySQL                                      |
| JDBC Driver | `mysql-connector-java-8.0.28.jar`          |
| Table Utils | `rs2xml.jar` for converting ResultSet to JTable |
| IDE         | IntelliJ IDEA                              |
| SDK         | Oracle OpenJDK 23 / Project SDK 20         |

---

##  Project Structure

Hospital Management System/
├── src/
│ ├── hospital/management/system/
│ │ ├── Login.java
│ │ ├── Reception.java
│ │ ├── NEW_PATIENT.java
│ │ ├── ALL_Patient_Info.java
│ │ ├── update_patient_details.java
│ │ ├── patient_discharge.java
│ │ ├── Room.java
│ │ ├── SearchRoom.java
│ │ ├── Employee_info.java
│ │ ├── Ambulance.java
│ │ ├── Department.java
│ │ ├── conn.java
│ └── icon/
│ ├── add.png
│ ├── advice.png
│ ├── ambulance.png
│ ├── patient.png
│ ├── patient1.png
│ ├── patient_discharge.png
│ ├── department.png
│ ├── logout.png
│ ├── project.png
│ ├── room.png
│ ├── roomm.png
│ ├── search.png
│ ├── Blue Professional Hospital Logo.png
├── README.md
├── workspace.xml

yaml
Copy
Edit

---

## 🗄 Database Schema

Here are the SQL tables used:

###  Tables
- `login(ID, PW)`
- `patient_info(ID, Number, Name, Gender, Patient_Disease, Room_Number, Deposit, Admission_Date)`
- `room(room_no, Availability, Price, Room_Type)`
- `department(Department, Phone_no)`
- `ambulance(ambulance_id, ambulance_type, status, contact_number)`
- `EMP_INFO(Name, Age, Phone_Number, Salary, Gmail, ID_Number)`

You can find the sample SQL insert statements in the `README.md` or `update_patient_details.java` file.

---

##  Dependencies

Make sure you’ve added the following JAR files to your classpath (as seen in **Project Structure > Modules > Dependencies**):

- [`mysql-connector-java-8.0.28.jar`](https://dev.mysql.com/downloads/connector/j/)
- `rs2xml.jar` – used to convert `ResultSet` to `JTable`

---

##  How to Run

1. Start your MySQL server and create the database:
   ```sql
   create database hospital_management_systems;
   use hospital_management_systems;
(Use the provided SQL script to create all tables.)

Open the project in IntelliJ IDEA.

Add the JDBC JAR files to the module dependencies.

Run Login.java to start the system.

📸 Sample UI

📚 Author
Haifa Afridi
Computer Engineering Student, NUST
First-Year Programming Project (2025)

🌟 Acknowledgements
Special thanks to our faculty for guidance.

Libraries: rs2xml.jar for JTable integration.

If you liked this project, feel free to ⭐ the repo!
