# Project Title: Library Management System using SQL

# Project Overview

This project implements a Library Management System using SQL with a structured relational database design. It simulates real-world library operations such as book issuance, returns, member management, and performance tracking.

The system demonstrates database design, data integrity enforcement, CRUD operations, stored procedures, and analytical reporting using SQL.

# Tools used
SQL (PostgreSQL),
Excel (for initial data preparation) and
DBMS (e.g., pgAdmin / MySQL Workbench)


# Database Design

The system consists of the following relational tables:

 branch – library branch details,
 employees – staff working in branches,
 members – library users,
 books – book inventory,
 issued_status – records of issued books and
 return_status – records of returned books
 
 Relationships
 
One branch → many employees,
One member → many issued books,
One book → multiple issue records,
Issue → Return mapping via issued_id


# Core Features
Data Management (CRUD Operations)

Insert, update, and delete records for books, members, and issue logs.

Manage book issue and return lifecycle.

Data Cleaning

Identified and handled NULL values across all tables.

Ensured data consistency after Excel import.

Transaction Workflow

Book issue and return tracking system.

Status update mechanism for availability control.




# Business Logic Implementation
A book can only be issued if its status is available

Upon return:

Entry is recorded in return_status

Book status is updated accordingly

Overdue books are identified using a 30-day return rule

# Analytical SQL Operations

The system supports advanced SQL-based reporting:

-> Overdue book detection (based on issue date logic)

-> Branch performance analysis (issues, returns, revenue)

-> Employee productivity tracking

-> Active member identification (last 2 months)

-> Book demand analysis using issue frequency

-> Revenue calculation by book category

# Advanced SQL Features Used
JOINs (INNER, LEFT JOIN)

GROUP BY & HAVING

Subqueries

CTAS (Create Table As Select)

Date functions (CURRENT_DATE, interval logic)

Stored Procedures (PL/pgSQL)

# Key Outcomes
Built a fully functional relational database system for library operations

Automated book issue/return workflow using stored procedures

Generated actionable insights from raw transactional data

Strengthened understanding of real-world database design principles

# How to Run This Project
Create database:

CREATE DATABASE library_db;

Run basic_queries.sql to create tables

Import Excel datasets into respective tables

advanced_queries.sql

# conclusion
This project demonstrates practical implementation of relational database design, transactional workflows, and analytical SQL querying in a real-world library system scenario.
