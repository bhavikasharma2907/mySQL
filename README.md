# mySQL
# Student Table (`dep1`) - MySQL Database Dump

## Overview

This repository contains a MySQL dump for the table **`dep1`** from the database **`bcd`**. The dump includes both the table schema and sample data for demonstration, backup, or migration purposes.

---

## Table Structure

The `dep1` table stores information about students and uses the following schema:

| Column   | Type         | Description              |
|----------|--------------|--------------------------|
| name     | varchar(30)  | Name of the student      |
| rollno   | int          | Student roll number      |
| grade    | varchar(10)  | Grade awarded (A/B/C/D)  |
| marks    | int          | Marks obtained           |

---

## Sample Data

Example records included in the dump file:

| name    | rollno | grade | marks |
|---------|--------|-------|-------|
| ash     | 1      | A     | 87    |
| kanishk | 2      | B     | 76    |
| soni    | 3      | A     | 89    |
| samina  | 4      | C     | 65    |
| asi     | 5      | B     | 64    |
| dfs     | 6      | C     | 56    |
| sdr     | 7      | D     | 42    |
| rgd     | 8      | A     | 99    |
| abz     | 9      | C     | 77    |
| lkj     | 10     | A     | 93    |

---

## How To Restore

To import the dump into your MySQL database:

mysql -u yourusername -p bcd < dep1_dump.sql

text

- Replace `yourusername` with your MySQL username.
- Make sure the target database `bcd` exists, or create it before running the command.

---

## Example SQL Queries

-- Display all students
SELECT * FROM dep1;

-- List students with grade 'A'
SELECT name, marks FROM dep1 WHERE grade = 'A';

-- Calculate the average marks
SELECT AVG(marks) FROM dep1;
