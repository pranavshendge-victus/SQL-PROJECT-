# SQL-PROJECT-
<br>
🚉 Project Overview — Railway Reservation System (SQL Project)

This SQL project simulates a Railway Reservation System, designed to manage passenger bookings, train details, payments, and journey information. It demonstrates the use of MySQL database design, data manipulation, and query operations — from basic selection to advanced aggregations and subqueries.

🧱 Database Structure

Database / Schema: railway_system

Main Table: Reservation

Reservation Table Columns:
Column Name	Description
Train_id	Unique ID of the train
Train_name	Name of the train
Train_type	Category (Express, Passenger, Superfast, etc.)
Coaches	Total number of coaches
PNR_no	Passenger PNR number
First_name / Last_name	Passenger name details
Contact / Email_id	Passenger contact info
Booking_id	Unique booking ID
Booking_date	Date of reservation
Source_station / Destination_station	Journey details
Seat_alloted	Seat or coach number
State / City	Passenger’s address info
Duration_minutes	Total travel duration
Payment_mode	Mode of payment (Online/Cash)
Fair	Ticket fare (price)
Booking_status	Status (Confirmed/Waiting)
Meal_booked	Boolean (True/False)
km	Distance travelled (added later)
Age	Passenger age (added later)
💾 Key Operations in the Project
1. Database Setup

Created schema railway_system

Created Reservation table and inserted multiple records

Added additional columns (km, Age) and updated data dynamically using CASE statements.

2. Basic SQL Queries

Selecting specific columns and all records

SELECT * FROM Reservation;
SELECT First_name, Last_name FROM Reservation;


Filtering records using WHERE, BETWEEN, and LIKE.

3. Aggregate Functions

Average, Count, Sum:

SELECT AVG(Fair) FROM Reservation;
SELECT COUNT(*) FROM Reservation;


Grouping and ordering:

SELECT Train_name, SUM(Fair) AS Total_Collection 
FROM Reservation
GROUP BY Train_name
ORDER BY Total_Collection DESC;

4. Conditional & Subqueries

Finding passengers with minimum age:

SELECT Age FROM Reservation WHERE Age = (SELECT MIN(Age) FROM Reservation);


IN, ANY, and EXISTS queries for advanced filtering.

5. String & Pattern Matching

Using LIKE, BETWEEN, and wildcard characters for flexible search.

6. High-Level Analytical Queries

Top trains by total revenue.

Average duration by train type.

Booking confirmation rate by train type.

Subqueries and conditional logic (CASE, HAVING, GROUP BY).

📊 Sample Insights Derived

Most common payment mode used by passengers.

Average travel duration by train category.

Trains generating highest total revenue (km * fare).

Booking confirmation rate across different train types.

Discount or insurance eligibility based on passenger age.

⚙️ SQL Concepts Covered

✅ DDL (CREATE, ALTER, DROP)
✅ DML (INSERT, UPDATE, DELETE)
✅ DQL (SELECT, WHERE, GROUP BY, ORDER BY)
✅ Aggregate & Scalar Functions (SUM, AVG, MAX, MIN)
✅ Subqueries & Nested SELECT
✅ CASE & Conditional Expressions
✅ Pattern Matching using LIKE & IN
✅ UNION & HAVING Clauses

🧩 Project Learning Goals

To understand relational database design.

To learn how to write optimized SQL queries for analytics.

To practice real-world data handling using MySQL.

To build a portfolio-ready SQL project for GitHub.

📝 What to Include in Your README on GitHub

Here’s what your README.md should contain:

# 🚉 Railway Reservation System (SQL Project)

### 📘 Overview
This SQL project simulates a Railway Reservation System that stores and manages passenger bookings, train details, and travel data using MySQL. It demonstrates SQL fundamentals, data analysis queries, and database design concepts.

---

### 🧱 Database Design
**Schema:** `railway_system`  
**Table:** `Reservation`

Key columns include Train details, Passenger info, Booking data, and Travel metrics.

---

### 🧰 Technologies Used
- MySQL
- SQL Workbench / phpMyAdmin
- Basic SQL to Advanced Analytical Queries

---

### 🔍 Features & Queries Covered
- Database & Table creation  
- Data Insertion & Updating  
- Aggregate functions (SUM, AVG, COUNT)  
- Grouping, Filtering, and Ordering  
- Subqueries and Nested SELECT statements  
- Conditional logic using CASE  
- Pattern matching with LIKE  
- UNION, HAVING, and LIMIT clauses  

---

### 📊 Insights Generated
- Train with highest total revenue  
- Most preferred payment mode  
- Average journey duration by train type  
- Confirmation vs Waiting booking ratio  
- Passenger discount/insurance eligibility by age  

---

### 💡 Learning Outcomes
- Strengthened SQL fundamentals  
- Real-world database design understanding  
- Hands-on experience with MySQL operations  
- Query optimization and logical problem solving  

---

### 🧾 Author
**Pranav Kumar Shendge**  
 
