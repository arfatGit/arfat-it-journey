# SQL Basics - Week 1

## What is a database?

A database is set of related data represented in tables.

## What is a table?

A table is consists of related data represented in rows and columns.

## What is a row?

A row also known as record is every entry of data in the table.

## What is a column?

A column is a group of data of same type

## What is a primary key?

A primary key is a unique data in a table that is used to filter data and is known as a target for the foreign key in another table. It can't be null.

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
