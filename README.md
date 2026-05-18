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

 -> branch – library branch details
 -> employees – staff working in branches
 -> members – library users
 -> books – book inventory
 -> issued_status – records of issued books
 -> return_status – records of returned books
 
 Relationships
One branch → many employees
One member → many issued books
One book → multiple issue records
Issue → Return mapping via issued_id

