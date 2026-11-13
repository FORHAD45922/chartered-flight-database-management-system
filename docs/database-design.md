# Database Design – Chartered Flight Database Management System

## 1. Introduction

This document describes the proposed database design for the Chartered Flight Database Management System (CFDBMS), developed for Impact Charter Services (ICS).

The database will provide a centralised structure for managing the company's operational information.

## 2. Database Requirements

The proposed database should support:

- Customer information management.
- Passenger information management.
- Charter flight bookings.
- Aircraft records.
- Pilot and crew records.
- Crew assignments.
- Financial transactions.
- Aircraft maintenance activities.

## 3. Proposed Database Entities

The proposed database will include the following entities:

1. Customer
2. Passenger
3. Booking
4. Flight
5. Aircraft
6. Pilot
7. Crew
8. Crew Assignment
9. Invoice
10. Payment
11. Maintenance

## 4. Database Relationships

The database will establish relationships between the entities:

- One customer can make multiple bookings.
- One booking can include multiple passengers.
- One aircraft can operate multiple flights.
- Pilots can be assigned to multiple flights.
- Crew members can be assigned to different flights.
- Each booking can generate an invoice.
- Each invoice can have associated payments.
- Aircraft can have multiple maintenance records.

## 5. Database Design Principles

The database design will follow these principles:

- Data integrity and consistency.
- Primary key and foreign key constraints.
- Reduction of data duplication.
- Appropriate database normalisation.
- Referential integrity.
- Efficient data retrieval.
- Secure data management.

## 6. Implementation Technologies

The project will use Oracle Database and SQL/PLSQL for database development, querying and management.

## 7. Project Status

Project Status: In Progress.

Further database development, SQL implementation, testing and documentation will be completed as part of the coursework.

## 8. Conclusion

The proposed CFDBMS will provide Impact Charter Services with a structured database solution to improve booking management, operational efficiency, data accuracy and information management.
