
```
SELECT emp_no, first_name, last_name, gender FROM employees limit 10;
```

```
SELECT emp_no, first_name, last_name, gender FROM employees ORDER BY last_name ASC LIMIT 10;
```

```
SELECT emp_no, first_name, last_name, gender FROM employees ORDER BY last_name ASC, first_name ASC LIMIT 10;
```

```
SELECT COUNT(emp_no) FROM employees WHERE last_name = 'Aamodt';
```

```
SELECT COUNT(emp_no) FROM employees;
```

```
SELECT last_name, COUNT(emp_no) AS num_emp FROM employees GROUP BY last_name ORDER BY num_emp DESC LIMIT 10;
```

```
SELECT COUNT(*) FROM salaries WHERE salary BETWEEN 60000 AND 70000;
```

```
SELECT employees.* FROM  employees 
LEFT JOIN dept_emp ON ( dept_emp.emp_no =  employees.emp_no ) 
LEFT JOIN salaries ON ( salaries.emp_no =  salaries.emp_no ) 
WHERE employees.first_name LIKE '%Jo%' 
AND salaries.from_date > '1993-01-21' 
AND salaries.to_date < '1998-01-01' LIMIT 0, 20;
```

More samples:
- https://www.ntu.edu.sg/home/ehchua/programming/sql/sampledatabases.html

