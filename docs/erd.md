# Entity Relationship Diagram (ERD)
## Chartered Flight Database Management System (CFDBMS)

## 1. Introduction

This document describes the proposed Entity Relationship Diagram (ERD) for the Chartered Flight Database Management System developed for Impact Charter Services (ICS).

The ERD identifies the main entities, their attributes, primary keys, foreign keys and relationships.

## 2. Database Entities

The proposed database includes the following entities:

1. Customer
2. Passenger
3. Booking
4. Flight
5. Aircraft
6. Pilot
7. Crew Member
8. Crew Assignment
9. Invoice
10. Payment
11. Maintenance

## 3. Primary Keys and Foreign Keys

| Entity | Primary Key | Foreign Key |
|---|---|---|
| Customer | CustomerID | - |
| Passenger | PassengerID | - |
| Booking | BookingID | CustomerID |
| Flight | FlightID | BookingID, AircraftID |
| Aircraft | AircraftID | - |
| Pilot | PilotID | - |
| Crew Member | CrewID | - |
| Crew Assignment | AssignmentID | FlightID, CrewID |
| Invoice | InvoiceID | BookingID |
| Payment | PaymentID | InvoiceID |
| Maintenance | MaintenanceID | AircraftID |

## 4. Entity Relationships

The proposed relationships include:

- One customer can make multiple bookings.
- One booking can contain multiple passengers.
- One booking can involve multiple flights.
- One aircraft can operate multiple flights.
- Pilots can be assigned to multiple flights.
- Crew members can work on multiple flights.
- One booking can generate an invoice.
- One invoice can have multiple payments.
- One aircraft can have multiple maintenance records.

## 5. Relationship Types

| Relationship | Type |
|---|---|
| Customer – Booking | One-to-Many |
| Booking – Passenger | Many-to-Many |
| Booking – Flight | One-to-Many |
| Aircraft – Flight | One-to-Many |
| Pilot – Flight | Many-to-Many |
| Crew Member – Flight | Many-to-Many |
| Booking – Invoice | One-to-One |
| Invoice – Payment | One-to-Many |
| Aircraft – Maintenance | One-to-Many |

## 6. Database Design Considerations

The database design will consider:

- Primary key constraints.
- Foreign key constraints.
- Referential integrity.
- Database normalisation.
- Reduction of duplicate data.
- Efficient data retrieval.
- Data consistency and accuracy.

## 7. Project Status

Project Status: In Progress.

The ERD will be reviewed and refined during the database implementation stage.

## 8. Conclusion

The proposed ERD provides a structured foundation for developing the Chartered Flight Database Management System. It establishes the relationships required to manage customers, bookings, passengers, flights, aircraft, pilots, crew, invoices, payments and maintenance records.
