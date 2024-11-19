# sql-challenge

This challenge was divided into three parts: data modeling, data engineering,
and data analysis.

For the data modeling part, http://www.quickdatabasediagrams.com/ was used to
create an Entity Relationship Diagram or ERD. 

For the data engineering part, six tables were created for six CSV files containing
information of people who were employed with the company during the 1980's and
1990's. 

When creating these tables, they were created in the following order: titles,
departments, employees, department_employees, department_managers, and salaries.

The reason for creating the 'titles' and 'departments' tables first is that they are
independent tables with no foreign key dependencies. The 'employees' table was
created next because it has a foreign key referencing the 'titles' table through the
'emp_title_id' column.

The 'department_employees' table was created next since it contains foreign keys
referencing both the 'employees' and 'departments' tables, requiring those to
already exist. Then the 'department_managers' and 'department_employees' tables 
were created next. Lastly the 'salaries' table was created.

For the data analysis part, a sql file containing queries was provided to answer the
following:

1. List the employee number, last name, first name, sex, and salary of each
employee.

2. List the first name, last name, and hire date for the employees who were hired in
1986.

3. List the manager of each department along with their department number,
department name, employee number, last name, and first name.

4. List the department number for each employee along witht that employee's 
employee number, last name, first name, and department name.

5. List the first name, last name, and sex of each employee whose first name is 
Hercules and whose last name begins with the letter B.

6. List each employee in the Sales department, including their employee number,
last name, and first name. 

7. List each employee in the Sales and Development departments, including their 
employee number, last name, first name, and department name. 

8. List the frequency counts, in descending order, of all the employee last names
(that is how many employees share each last name).

