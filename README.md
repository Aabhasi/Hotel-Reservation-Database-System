
# 🏨 Hotel Reservation System Database

This project presents a structured **Hotel Reservation System Database** built using SQL to manage and streamline key hotel operations such as room bookings, guest services, payments, and reservations. It was developed as part of a team-based MIS 632 project.

## 🎯 Project Objectives
- Design a relational database to manage hotel reservations, rooms, guests, and payment processes.
- Ensure data integrity, reduce redundancy, and enable scalable operations.
- Support hotel staff in efficient reservation management and financial reporting.

## 🛠️ Tools & Technologies
- **SQL (Oracle & SQL Server compatible)**
- **ER Diagram Design**
- **Oracle APEX** 
- Relational schema development with primary/foreign keys and constraints

## 🧩 Features & Entities
- **ROOM**: Tracks room number, type, rate, and bed configuration
- **ROOMTYPE**: Classifies rooms into Standard, Deluxe, Suite, etc.
- **GUEST**: Maintains guest contact information
- **RESERVATION**: Handles check-in/check-out, room booking, and total amount
- **PAYMENT**: Stores method, amount paid, and pending dues

## 📈 Business Insights Enabled
- Track occupancy rates and booking trends by room type
- Analyze total revenue by payment method
- Identify high-revenue rooms and booking durations

## ✅ Key Achievements
- Ensured **data consistency** using entity relationships and constraints
- **Improved operational efficiency** through automation
- Enabled **scalable and secure** reservation processing

## 💡 Sample Business Queries
```sql
-- 1. Occupancy Rate Analysis
SELECT roomid, COUNT(*) AS bookings, SUM(totalamount) AS revenue
FROM reservation
GROUP BY roomid
ORDER BY bookings DESC;

-- 2. Revenue by Payment Method
SELECT paymentmethod, SUM(paidamount) AS total_paid
FROM payment
GROUP BY paymentmethod;
```

This database supports day-to-day hotel operations while enabling data-driven decisions to boost profitability and guest satisfaction.
