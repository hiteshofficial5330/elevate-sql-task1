# Elevate Labs - SQL Developer Internship Task 1

## Task Overview
This project is the first task for the SQL Developer Internship at Elevate Labs. The objective is to design and set up a database schema for an E-commerce domain. This includes creating the tables, defining relationships, and generating an ER diagram.

- **Domain:** E-commerce
- **Tools Used:** MySQL Workbench

---

## Schema Design
The database `ecommerce_db` consists of four tables designed to handle customers, products, and their orders efficiently through normalization. The complete SQL script for creating this schema is available in the `schema.sql` file.

---

## ER Diagram
The following ER Diagram illustrates the schema design, including table attributes and the one-to-many and many-to-many relationships.

![ER Diagram for E-commerce DB](ER_Diagram.png)

---

## Theoretical Questions & Answers

### 1. What is normalization?
Normalization is the process of organizing columns and tables in a relational database to minimize data redundancy and improve data integrity.

### 2. Explain primary vs foreign key.
A **Primary Key** uniquely identifies each record in a table (e.g., `CustomerID`). A **Foreign Key** is a field in one table that refers to the Primary Key in another table, creating a link between them (e.g., the `CustomerID` in the `Orders` table).

### 3. What are constraints?
Constraints are rules applied to data columns to ensure data accuracy. Examples include `NOT NULL`, `UNIQUE`, `PRIMARY KEY`, and `FOREIGN KEY`.

### 4. What is a surrogate key?
A surrogate key is an artificially generated unique ID (like an `AUTO_INCREMENT` integer) that has no business meaning. Its sole purpose is to be the primary key.

### 5. How do you avoid data redundancy?
Data redundancy is avoided primarily through normalization, which involves splitting large tables into smaller, related ones so that each piece of information is stored only once.

### 6. What is an ER diagram?
An ER diagram is a visual flowchart that shows the database's entities (tables), their attributes (columns), and the relationships between them.

### 7. What are the types of relationships in DBMS?
The main types are One-to-One (1:1), One-to-Many (1:N), and Many-to-Many (M:N).

### 8. Explain the purpose of AUTO_INCREMENT.
`AUTO_INCREMENT` automatically generates a unique number for a column when a new row is added, which is perfect for creating surrogate primary keys.

### 9. What is the default storage engine in MySQL?
The default storage engine in modern MySQL versions is **InnoDB** because it supports transactions and foreign keys, ensuring data integrity.

### 10. What is a composite key?
A composite key is a primary key made up of two or more columns combined to uniquely identify a record.
