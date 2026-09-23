# College Enrollment System — Dataase Design
ada
A relational database design for a college enrollment system, created for the assignment:
**"Create relational databases and tables using SQL for a college enrollment system."**

## What's included

Open `college_enrollment_system.html` in any web browser. It contains:

1. **ERD Diagram** — a visual entity-relationship diagram showing all 9 tables, their attributes, data types, and how they connect (primary keys, foreign keys, and 1-to-many relationships).
2. **Database Schema (SQL DDL)** — `CREATE TABLE` statements for every table, with appropriate SQL data types (`INT`, `VARCHAR(n)`, `DATE`), `PRIMARY KEY`, `FOREIGN KEY`, and `NOT NULL` constraints.
3. **Relationship Summary** — a quick-reference table listing every parent → child relationship and the foreign key that enforces it.

## Tables

| Table | Purpose |
|---|---|
| department | Academic departments |
| semester | Academic terms |
| program | Degree programs, linked to a department |
| instructor | Teaching staff, linked to a department |
| course | Courses offered, linked to a department |
| student | Enrolled students, linked to a program |
| course_offering | A specific course taught in a specific semester by a specific instructor |
| enrollment | Links students to the course offerings they're enrolled in |

## How to use

- Double-click `college_enrollment_system.html` to view it in your browser — no installation needed.
- Copy the SQL from the schema section directly into MySQL, PostgreSQL, or any SQL-compatible tool to create the tables.
- Run the `CREATE TABLE` statements in this order (parents before children): department → semester → program → instructor → course → student → course_offering → enrollment.
