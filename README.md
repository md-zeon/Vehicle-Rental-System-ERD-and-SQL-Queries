# Vehicle Rental System – Database ERD Design and SQL Queries

## 1. Project Overview
This project focuses on the design and implementation of a **Vehicle Rental System database**. The primary objective is to develop a relational database schema that accurately reflects real-world business requirements and to perform SQL queries to extract meaningful insights.

The project demonstrates the application of **relational database concepts**, including entity-relationship modeling, primary and foreign key constraints, and various SQL querying techniques.

---

## 2. Learning Objectives
Upon completion of this project, the following competencies are demonstrated:

- Designing an **Entity Relationship Diagram (ERD)** with appropriate relationships
- Defining **Primary Keys (PK)** and **Foreign Keys (FK)** to ensure data integrity
- Writing SQL queries utilizing:
  - `INNER JOIN`
  - `NOT EXISTS`
  - `WHERE`
  - `GROUP BY` and `HAVING`
- Applying business rules and constraints in a real-world database scenario

---

## 3. System Modules
The system comprises three core entities:

1. **Users** – representing administrators and customers  
2. **Vehicles** – representing available rental vehicles, including cars, bikes, and trucks  
3. **Bookings** – representing rental records that connect users with vehicles

---

## 4. Database Design (ERD)

### 4.1 Tables
- `users`  
- `vehicles`  
- `bookings`  

### 4.2 Relationships
- **One-to-Many:** One user can have multiple bookings  
- **Many-to-One:** Multiple bookings may reference the same vehicle  
- **Logical One-to-One:** Each booking is associated with exactly one user and one vehicle  

### 4.3 Features
- Primary Keys (PK) and Foreign Keys (FK)  
- Relationship cardinality clearly defined  
- Status fields such as booking status and vehicle availability included  

### 4.4 ERD Tool
The ERD was created using **drawSQL**:  
[Vehicle Rental System ERD](https://drawsql.app/teams/developer-zeon/diagrams/vehicle-rental-system)

---

## 5. Repository Structure
/Vehicle-Rental-System-ERD-and-SQL-Queries
│
├── README.md
├── QUERIES.sql

---

## 6. SQL Queries

### Query 1: INNER JOIN
**Objective:** Retrieve booking details including customer name and vehicle name.  
**Concept Used:** `INNER JOIN`  
**Description:** This query joins the `bookings`, `users`, and `vehicles` tables to provide comprehensive booking information.

---

### Query 2: NOT EXISTS
**Objective:** Identify all vehicles that have never been booked.  
**Concept Used:** `NOT EXISTS`  
**Description:** This query filters vehicles whose IDs do not appear in the `bookings` table, ensuring only unbooked vehicles are returned.

---

### Query 3: WHERE Clause
**Objective:** Retrieve all available vehicles of a specific type (e.g., cars).  
**Concept Used:** `WHERE`  
**Description:** This query applies filters on vehicle type and availability status to extract only relevant records.

---

### Query 4: GROUP BY and HAVING
**Objective:** Determine vehicles that have been booked more than twice.  
**Concepts Used:** `GROUP BY`, `HAVING`, `COUNT`  
**Description:** This query groups bookings by vehicle and filters results to include only those vehicles with more than two bookings.

---

## 7. Theory Component (Viva Practice)
The theory component aims to evaluate comprehension of fundamental database concepts.  
Responses were recorded in **English** for viva practice.

**Topics Covered:**
- Definition and importance of a **foreign key**
- Differences between `WHERE` and `HAVING` clauses
- Definition and characteristics of a **primary key**
- Difference between `INNER JOIN` and `LEFT JOIN`

---

## 8. References and Links
- **GitHub Repository:** [Github Repo](https://github.com/md-zeon/Vehicle-Rental-System-ERD-and-SQL-Queries)  
- **ERD Diagram:** [Vehicle Rental System ERD](https://drawsql.app/teams/developer-zeon/diagrams/vehicle-rental-system)  
- **Video Link:** [Google Drive](https://drive.google.com/file/d/1PHAMqRDwGjSOvT5ZMWG6ydJdqvYJW1Pn/view?usp=drivesdk)

---

## 9. Conclusion
This project demonstrates the practical application of **relational database design** principles and **SQL query** in the context of a Vehicle Rental System. The database schema ensures data integrity, supports real-world business rules, and enables retrieval of actionable information through structured queries.
