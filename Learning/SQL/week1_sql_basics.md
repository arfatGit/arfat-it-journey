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

| employee_id | name    | department | role            | city     |
| ----------- | ------- | ---------- | --------------- | -------- |
| 1           | Arfatul | IT         | Support Analyst | Ottawa   |
| 2           | Sara    | HR         | Manager         | Toronto  |
| 3           | David   | Finance    | Analyst         | Ottawa   |
| 4           | Nina    | IT         | Developer       | Ottawa   |
| 5           | Omar    | Operations | Coordinator     | Montreal |

SELECT \* FROM employees;

SELECT name, department FROM employees;

SELECT \* FROM employees
WHERE department = 'IT';

SELECT \* FROM employees
WHERE city = 'Ottawa';

SELECT \* FROM employees
ORDER BY name;

SELECT \* FROM employees
ORDER BY department;

## Application Support Use Case

In an application support role, SQL can help investigate issues such as:

- finding a user's account
- checking ticket status
- finding incomplete records
- checking which department submitted the most tickets
- identifying old unresolved tickets

Example:

SELECT \* FROM tickets
WHERE status = 'Open';

SELECT \* FROM tickets
WHERE priority = 'High'
ORDER BY created_date;

## Example Table: tickets

| ticket_id | user_name | department | category       | priority | status      | created_date |
| --------- | --------- | ---------- | -------------- | -------- | ----------- | ------------ |
| 101       | Sara      | HR         | Login          | High     | Open        | 2026-06-20   |
| 102       | David     | Finance    | Report Error   | Medium   | In Progress | 2026-06-21   |
| 103       | Nina      | IT         | Access Request | Low      | Closed      | 2026-06-22   |
| 104       | Omar      | Operations | System Error   | High     | Open        | 2026-06-19   |

### Practice queries

-- Show all open tickets
SELECT \* FROM tickets
WHERE status = 'Open';

-- Show high priority tickets
SELECT \* FROM tickets
WHERE priority = 'High';

-- Show tickets from HR
SELECT \* FROM tickets
WHERE department = 'HR';

-- Show tickets ordered by created date
SELECT \* FROM tickets
ORDER BY created_date;
-- Show only ticket_id, user_name, and status
SELECT ticket_id, user_name, status FROM tickets;

## What I Learned

- A database stores related data in tables.
- A table is made of rows and columns.
- A primary key uniquely identifies each row.
- SELECT is used to choose data from a table.
- WHERE is used to filter records.
- ORDER BY is used to sort results.
