# SQL Practical Labs

**Course:** Google Cybersecurity Professional Certificate  
**Module:** Tools of the Trade: Linux and SQL  
**Environment:** MariaDB

## Overview

Completed hands-on SQL labs using a simulated organizational database, focusing on data retrieval, sorting, filtering, and combining relational tables. The activities involved investigating login attempts, identifying employee devices requiring security updates, and retrieving security-related information.

## Completed Labs

### 1. Perform SQL Queries

- Retrieved employee device information.
- Selected specific columns containing operating systems and patch dates.
- Investigated login activity.
- Sorted login attempts chronologically.

**Example SQL Queries:**

```sql
SELECT device_id, operating_system, OS_patch_date
FROM machines;
```

```sql
SELECT *
FROM log_in_attempts
ORDER BY login_date, login_time;
```

The first query retrieves device and patch information. The second sorts login attempts by date and time.

**SQL Keywords:** `SELECT`, `FROM`, `ORDER BY`

### 2. Apply Basic Filters to SQL Queries

- Identified machines running OS 2 that required updates.
- Retrieved employees from specific departments.
- Identified employees located in the South building.

**Example SQL Queries:**

```sql
SELECT device_id, operating_system
FROM machines
WHERE operating_system = 'OS 2';
```

```sql
SELECT *
FROM employees
WHERE office LIKE 'South%';
```

The `WHERE` clause filters records based on specific conditions. The `LIKE` operator uses `%` to match office names beginning with `South`.

**SQL Keywords:** `WHERE`, `LIKE`

### 3. Apply More Filters to SQL Queries

- Retrieved login attempts after a specified date.
- Filtered login attempts within a date range.
- Investigated attempts occurring at a specific time.
- Retrieved records using unique login identifiers.

**Example SQL Queries:**

```sql
SELECT *
FROM log_in_attempts
WHERE login_date > '2023-01-15';
```

```sql
SELECT *
FROM log_in_attempts
WHERE login_date BETWEEN '2023-02-01' AND '2023-02-07';
```

```sql
SELECT *
FROM log_in_attempts
WHERE login_time = '09:30:00';
```

These queries demonstrate date comparisons, inclusive date ranges, and exact time matching.

**SQL Operators:** `=`, `>`, `BETWEEN`

### 4. Filter with AND, OR, and NOT

- Identified failed login attempts occurring after business hours.
- Investigated login activity on specific dates.
- Retrieved login attempts originating outside Mexico.
- Identified employees requiring security updates.

**Example SQL Queries:**

```sql
SELECT *
FROM log_in_attempts
WHERE login_time > '18:00'
AND success = FALSE;
```

This query retrieves failed login attempts occurring after 18:00.

```sql
SELECT *
FROM log_in_attempts
WHERE login_date = '2022-05-09'
OR login_date = '2022-05-08';
```

The `OR` operator retrieves records matching either date.

```sql
SELECT *
FROM log_in_attempts
WHERE NOT country LIKE 'MEX%';
```

The `NOT` operator excludes login attempts with country values beginning with `MEX`.

```sql
SELECT *
FROM employees
WHERE department = 'Marketing'
AND office LIKE 'East%';
```

This query retrieves Marketing employees located in the East building.

**SQL Operators:** `AND`, `OR`, `NOT`, `LIKE`

### 5. Combine Tables Using SQL Joins

- Matched employees with their assigned machines.
- Retrieved all machines, including those without assigned employees.
- Retrieved employee records regardless of machine assignment.
- Connected employee information with login attempt records.

**Example SQL Queries:**

```sql
SELECT *
FROM machines
INNER JOIN employees
ON machines.device_id = employees.device_id;
```

An `INNER JOIN` returns records with matching device IDs in both tables.

```sql
SELECT *
FROM machines
LEFT JOIN employees
ON machines.device_id = employees.device_id;
```

A `LEFT JOIN` returns all machines, including those without matching employee records.

```sql
SELECT *
FROM machines
RIGHT JOIN employees
ON machines.device_id = employees.device_id;
```

A `RIGHT JOIN` returns all employee records, including employees without matching machine records.

```sql
SELECT *
FROM employees
INNER JOIN log_in_attempts
ON employees.username = log_in_attempts.username;
```

This query connects employee information with corresponding login attempt records.

**SQL Keywords:** `INNER JOIN`, `LEFT JOIN`, `RIGHT JOIN`, `ON`

## Skills Practiced

- SQL data retrieval and sorting.
- Filtering security-related records using conditional operators.
- Date and time-based investigation.
- Pattern matching using `LIKE`.
- Identifying failed login attempts.
- Retrieving employee and device information.
- Combining relational tables using SQL joins.
- Supporting security investigations through database queries.

---

*Completed as part of the Google Cybersecurity Professional Certificate using a simulated organizational database. SQL examples are drawn from the course labs.*
