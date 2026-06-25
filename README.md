# Online Donation Management System

## Overview

The Online Donation Management System is a database management project developed using MySQL. It provides a centralized platform for managing donors, organizations, donations, and payment transactions. The system helps charitable organizations and NGOs maintain donation records efficiently while ensuring transparency and accountability.

## Features

* Donor Registration and Management
* Organization Management
* Online Donation Tracking
* Payment Management
* Donation History Records
* Secure Storage of Transaction Details
* Support for Multiple Organizations
* SQL Queries for Data Analysis
* Advanced SQL Features (Views, Procedures, Triggers)

## Database Design

### Entities

1. **Donor**

   * donor_id (Primary Key)
   * name
   * email
   * phone

2. **Organization**

   * org_id (Primary Key)
   * name
   * type
   * address

3. **Donation**

   * donation_id (Primary Key)
   * amount
   * date
   * donor_id (Foreign Key)
   * org_id (Foreign Key)

4. **Payment**

   * payment_id (Primary Key)
   * method
   * status
   * donation_id (Foreign Key)

### Relationships

* One Donor can make multiple Donations (1:M)
* One Organization can receive multiple Donations (1:M)
* One Donation has one Payment record (1:1)

## Technologies Used

* MySQL
* SQL
* DBMS Concepts
* ER Modeling
* Normalization (3NF & BCNF)

## Project Structure

```
Online-Donation-Management-System/
│
├── SQL/
│   ├── create_tables.sql
│   ├── insert_data.sql
│   ├── queries.sql
│   └── advanced_features.sql
│
├── ER_Diagram/
│   └── er_diagram.png
│
├── Documentation/
│   └── Project_Report.pdf
│
└── README.md
```

## Sample SQL Queries

* List all donors
* Calculate total donation amount
* Find donations with donor names
* Count donations received by each organization
* Display payment details with donation amounts
* Find highest and lowest donation amounts

## Advanced SQL Features

### View

Displays donor names along with donation amounts.

### Stored Procedure

Retrieves donation information efficiently.

### Trigger

Automatically performs actions before data insertion.

## Results

The system successfully:

* Maintains donor, organization, donation, and payment records.
* Enforces relationships using primary and foreign keys.
* Reduces data redundancy through normalization.
* Executes SQL queries accurately.
* Implements advanced database features such as views, procedures, and triggers.

## Future Enhancements

* Web-based user interface
* Payment gateway integration
* Admin dashboard
* Mobile application support
* Real-time donation analytics

## Learning Outcomes

This project demonstrates:

* Database design using ER models
* Relational schema creation
* SQL query implementation
* Database normalization
* Use of advanced SQL features
* Real-world application of DBMS concepts

