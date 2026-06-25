# SQL Basics - Week 1

## What is a database?

A database is a collection of related data, usually organized into tables.

## What is a table?

A table stores related data in rows and columns.

## What is a row?

A row, also called a record, represents one entry in a table.

## What is a column?

A column represents one type/category of data in a table, such as name, department, or role.

## What is a primary key?

A primary key is a column, or group of columns, that uniquely identifies each row in a table. It cannot be null, and it can be referenced by a foreign key in another table.

## Example Employee Table

| employee_id | name    | department | role            |
| ----------- | ------- | ---------- | --------------- |
| 1           | Arfatul | IT         | Support Analyst |
| 2           | Sara    | HR         | Manager         |
| 3           | David   | Finance    | Analyst         |

## Practice Queries

SELECT \* FROM employees;

SELECT name, department FROM employees;

SELECT \* FROM employees
WHERE department = 'IT';

SELECT \* FROM employees
ORDER BY name;

## What I Learned

- A database stores related data in tables.
- A table is made of rows and columns.
- A primary key uniquely identifies each row.
- SELECT is used to choose data from a table.
- WHERE is used to filter records.
- ORDER BY is used to sort results.
