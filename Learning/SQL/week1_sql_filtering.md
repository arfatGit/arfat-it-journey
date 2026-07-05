# SQL Filtering Practice

## Ticket Table

| ticket_id | user_name | department | category       | priority | status      | created_date |
| --------- | --------- | ---------- | -------------- | -------- | ----------- | ------------ |
| 101       | Sara      | HR         | Login Issue    | High     | Open        | 2026-06-20   |
| 102       | David     | Finance    | Report Error   | Medium   | In Progress | 2026-06-21   |
| 103       | Nina      | IT         | Access Request | Low      | Closed      | 2026-06-22   |
| 104       | Omar      | Operations | System Error   | High     | Open        | 2026-06-19   |
| 105       | Maya      | HR         | Password Reset | Medium   | Closed      | 2026-06-18   |
| 106       | James     | Finance    | Login Issue    | High     | Open        | 2026-06-22   |
| 107       | Laila     | Operations | Access Request | Low      | Open        | 2026-06-23   |

-- 1. Show all open tickets

    select ticket_id from Ticket
    where status = 'Open';

-- 2. Show all high priority open tickets

    select ticket_id from Ticket
    where priority = 'High' and status = 'Open';

-- 3. Show tickets from HR or Finance

    select ticket_id from Ticket
    where department = 'HR' or department = 'Finance';

-- 4. Show tickets where category contains "Login"

    select ticket_id from Ticket
    where category like '%Login%'

-- 5. Show tickets where category contains "Error"

    select ticket_id from Ticket
    where category like '%Error%';

-- 6. Show tickets created between 2026-06-19 and 2026-06-22

    select ticket_id from Ticket
    where created_date between '2026-06-19' and '2026-06-22';

-- 7. Count all tickets

    select count(ticket_id) from Ticket;

-- 8. Count tickets by department

    select department, count(ticket_id) as ticket_count from Ticket
    group by department;

-- 9. Count tickets by status

    select status, count(ticket_id) as ticket_count from Ticket
    group by status;

-- 10. Show open tickets ordered by created_date

    select ticket_id from Ticket
    where status = 'Open'
    order by created_date;
