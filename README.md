# SQL-Intern-task-3
Task 3: Writing Basic SELCET Queries
##  Objectives 
The goal of task is to **extract data from one ot more tables** using SQL 'SELECT' queries, including filtering, sorting, and limiting the results.
## Tools Used
**DB Browser for SQLite** / **MySQL Workbench**
## Table Used 
Creating the sample table employees
      CREATE TABLE employees (
          emp_id INTEGER PRIMARY KEY,
          name VARCHAR(50),
          department VARCHAR(50),
          salary REAL,
          hire_date DATE
          );
sample date inserted :
  INSERT INTO employees (emp_id, name, department, salary, hire_date) VALUES ( 1, 'Alice' , 'HR' , 40000 , '2022-01-15');

 ** 1. SELECT ALL Specific Columns**
   
  SELECT * FROM employees;
  SELECT name,department FROM employees;

 **2. Filtering with WHERE, AND, OR, LIKE, BETWEEN**
    
SELECT * FROM employees WHERE department = 'IT';
SELECT * FROM employees WHERE department = 'HR' AND salary > 40000;
SELECT * FROM employees WHERE department = 'IT' OR department = 'Finance';
SELECT * FROM employees WHERE name LIKE 'A%';
SELECT * FROM employees WHERE salary BETWEEN 45000 AND 70000;

**3.Sorting Results**

ORDER BY salary ASC
ORDER BY name DESC

**4.Limiting Results**

LIMIT 3 to show top 3 results

OUTCOME:

Use basic SELECT queries to retrieve full or partial data.
Apply conditional filters using WHERE, AND, OR, LIKE, and BETWEEN.
Sort results using ORDER BY.
Limit output using LIMIT.
