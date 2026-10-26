🩸 Quick Blood

Smart Blood Donation \& Donor Management System

Quick Blood is a Blood Donation \& Donor Management System designed to efficiently manage donors, recipients, hospitals, blood banks, donations, blood inventory, and emergency blood requests through a centralized MySQL database.



The system helps healthcare organizations maintain accurate blood records, track donations, manage inventory, and fulfill blood requests quickly and efficiently.



🎯 Project Objective

The main objective of Quick Blood is to provide a centralized platform to:



Register and manage blood donors

Maintain recipient information

Manage blood banks and hospitals

Track blood donations

Monitor blood inventory

Process blood requests

Improve blood availability management

Maintain data accuracy and consistency

The system is designed to support real-world blood donation activities and emergency blood requirements.



🏥 System Modules

👨‍🦰 Donor Management

The donor module stores:



Donor Details

Blood Group

Contact Information

Donation History

City Information

🧑 Patient \& Recipient Management

Recipients can:



Register blood requirements

Submit blood requests

Track request status

Connect with hospitals

🏨 Hospital Management

Hospitals can:



Raise blood requests

Track request approvals

Receive blood from blood banks

Maintain request records

🩸 Blood Bank Management

Blood banks can:



Maintain inventory

Accept donations

Fulfill requests

Monitor blood stock levels

📦 Blood Inventory Management

The inventory module manages:



Blood Group Availability

Blood Stock Information

Available Units

Blood Bank Storage Records

👥 User Roles

🩸 Donor

A donor can:



Donate blood

Maintain donation records

Check donation history

🏥 Hospital

A hospital can:



Request blood units

Track request status

Receive blood from blood banks

🏦 Blood Bank

A blood bank can:



Manage blood stock

Accept donations

Process requests

Supply blood to hospitals

🔐 Administrator

The administrator manages:



Donors

Recipients

Hospitals

Blood Banks

Blood Inventory

Donations

Requests

🗄️ Database Design

The project is built using MySQL and consists of multiple interconnected tables.



Core Tables

Table Name	Purpose

blood\_groups	Stores blood group details

donors	Stores donor information

recipients	Stores recipient data

hospitals	Stores hospital information

blood\_banks	Stores blood bank details

donations	Stores donation records

blood\_inventory	Stores blood stock details

requests	Stores blood requests

donation\_log	Stores donation logs

🔗 Database Features

✅ Tables

The system uses relational database tables to store and manage blood donation information.



✅ Primary Keys \& Foreign Keys

Used to maintain relationships between:



Donors

Recipients

Hospitals

Blood Banks

Donations

Requests

Inventory

✅ Indexes

Indexes improve database performance for frequently searched data.



Examples:



Donor Blood Group

Request Status

Hospital Information

Blood Bank Records

✅ Views

The system includes reusable views:



view\_donor\_details

Displays:



Donor Name

Blood Group

City

Last Donation Date

view\_blood\_stock

Displays:



Blood Bank Name

Blood Group

Available Units

view\_donation\_history

Displays:



Donation Details

Donor Information

Blood Bank Information

view\_pending\_requests

Displays all pending blood requests.



view\_total\_donations

Displays donor-wise total donations.



view\_request\_fulfilment

Displays request fulfillment information.



✅ Stored Procedures

The project contains reusable stored procedures:



sp\_get\_donor\_history()

sp\_available\_blood()

sp\_pending\_requests()

sp\_donors\_by\_city()

sp\_bloodbank\_stock()

sp\_approve\_request()

Features

Search donor history

Check blood availability

Find pending requests

Search donors by city

Check blood bank stock

Approve requests

✅ Triggers

Automatic triggers are used for maintaining data integrity.



Implemented Triggers

trg\_log\_donation

Automatically logs donations.



trg\_add\_stock\_on\_donation

Updates inventory when blood is donated.



trg\_reduce\_stock\_on\_complete

Reduces stock after request completion.



trg\_prevent\_negative\_units

Prevents inventory values from becoming negative.



📊 Query Bank

The project contains SQL queries categorized into multiple levels.



Level 1 – Simple Queries

Examples:



Display donors

Display blood banks

Display pending requests

Level 2 – Intermediate Queries

Examples:



Donation details

Blood availability reports

Donor count by city

Level 3 – Complex Queries

Examples:



Top Donor Analysis

Blood Stock Analysis

Request Fulfillment Reports

🧩 Entity Relationship Diagram

The system follows the relationship model below:



Blood Groups

&#x20;     ↓

&#x20;   Donors

&#x20;     ↓

&#x20; Donations

&#x20;     ↓

&#x20;Blood Banks

&#x20;     ↓

Blood Inventory





Recipients

&#x20;     ↓

&#x20;  Requests

&#x20;     ↓

&#x20; Hospitals

&#x20;     ↓

&#x20;Blood Banks

The complete ER Diagram is included in the repository.



🛠️ Technologies Used

Database

MySQL

MySQL Workbench

📁 Project Structure

Quick-Blood/

│

├── quick\_blood\_db\_.txt

├── Quick\_Blood\_ER\_Diagram.png

└── README.md

quick\_blood\_db\_.txt

Contains:



Database Creation

Table Creation

Sample Data

Indexes

Views

Stored Procedures

Triggers

Query Bank

Quick\_Blood\_ER\_Diagram.png

Contains:



Complete Entity Relationship Diagram

🚀 Future Development

Phase 1 — Database ✅

Database Design

ER Diagram

Table Creation

Sample Data

Indexes

Views

Stored Procedures

Triggers

Phase 2 — Python Backend

MySQL Connectivity

Business Logic

Service Layer

Phase 3 — Flask REST API

Authentication

Donor APIs

Recipient APIs

Blood Bank APIs

Hospital APIs

Request APIs

Phase 4 — Frontend

React Application

Dashboard

Donor Management

Inventory Management

Request Tracking

Phase 5 — Full Stack Integration

React Frontend

&#x20;     ↓

&#x20;Flask REST API

&#x20;     ↓

&#x20;Python Backend

&#x20;     ↓

&#x20;MySQL Database

🔒 Data Integrity \& Security

The database implements:



Foreign Key Constraints

Data Validation

Trigger-Based Protection

Inventory Control

Transaction Safety

Future application development will include:



Authentication

Authorization

Password Hashing

Secure API Access

**📌 Project Status**

Current Stage: MySQL Database Development ✅

The database schema, tables, relationships, sample data, indexes, views, stored procedures, triggers, and query bank have been successfully implemented.



Future development will extend the system into a complete:



Python + Flask + React Full-Stack Application



👨‍💻 Developer

Ratnala Deepak

Project: Quick Blood - Smart Blood Donation \& Donor Management System



⭐ Project Vision

Quick Blood aims to bridge the gap between donors, blood banks, hospitals, and recipients through a reliable, scalable, and efficient blood donation management platform.

