# Hotel Management System

## Overview
A complete Database Management System for hotel operations.
This system manages hotel chains, rooms, bookings, guests,
employees, departments and services through a structured
and normalized MySQL database.

---

## Features
- Hotel chains and their details management
- Room booking and reservations
- Guest check-in and check-out
- Billing and payment management
- Employee and department records
- Hotel services tracking
- Database Views and Triggers for automation

---

## Database Design

### Tables:
| Table | Description |
|---|---|
| bookings | Manages all room booking records |
| guests | Stores guest information |
| employees | Manages employee records |
| rooms_booked | Tracks booked rooms per booking |
| department | Hotel department information |
| addresses | Address info for guests, hotels, employees |
| hotel_services_used_by_guests | Services used by guests |

### Relationships:
- Bookings → Hotels (Many to One)
- Bookings → Guests (Many to One)
- Employees → Departments (Many to One)
- Employees → Hotels (Many to One)
- Rooms Booked → Bookings (Many to One)

---

## Database Normalization
Database is normalized up to Third Normal Form (3NF) to:
- Reduce data redundancy
- Improve data integrity
- Make data easily accessible

---

## Views Created
- **GuestsDetails** — Shows complete information about guests
- **EmployeeDetails** — Shows employee info with their departments

---

## Triggers Created
- **BookingAudit_OnInsert** — Creates audit record when new 
  booking is added
- **BookingAudit_OnDelete** — Creates audit record when a 
  booking is deleted

---

## Technologies Used
- **Database:** MySQL
- **Frontend:** HTML
- **Tools:** MySQL Workbench

---

## How to Run
1. Import the SQL file into MySQL Workbench
2. Run the database schema to create all tables
3. Execute the queries to test the system
4. Open HTML file in browser for frontend

---

## Applications
- Hotel chain management
- Room booking and reservation system
- Guest and employee record management
- Automated booking audit system

---

## Contact
Wajeeha Attiq  
GitHub: github.com/wajeehaattiq  
Email: wajeehaattiq7@gmail.com
