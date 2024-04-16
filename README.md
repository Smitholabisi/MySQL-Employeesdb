# MySQL-Employees DATABASE 

## Retrieving Employees information 

creating databases, use the databases, DDL, DML, databases management skills, SQL proficiency and understanding of real- world applications.

-- 1 show all the columns and rows in the table

Select dept_no
from departments;

-- 2 show all the first name and last name 
select first_name, Last_name
from employees;

-- 3 Retrieve a list with all female employees whose first name is Kellie
select *
from employees
where first_name = 'kellie' and Gender = 'f' ;


-- 4. Retrieve a list with all employees whose first name is either Kellie or Aruna. 
select *
from employees 
where first_name = 'kellie' or first_name = 'Aruna';

-- 5. Select all the information from the “salaries” table regarding contracts from 66,000 to 70,000 dollars per year.

select * from salaries
where salary between 66000 and 70000;


-- 6. Retrieve a list with data about all female employees who were hired in the year 2000 or after.

select * from employees 
where hire_date >= '2000-01-01' 
and gender = 'f' ;

-- 7. Extract a list with all employees’ salaries higher than $150,000 per annum.
select * from salaries
where salary > 150000 ;

-- 8. Obtain a list with all different “hire dates” from the “employees” table
select distinct hire_date
from employees ;

