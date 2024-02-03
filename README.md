# SQL-Case-Study2

Query writing:

C:\Users\patil>cd\

C:\>cd xampp\mysql\bin

C:\xampp\mysql\bin>mysql -h localhost -u root

MariaDB [(none)]> use college;


Create Tables and Insert values:

create table employeedate(employee_id int AUTO_INCREMENT = 100, first_name
varchar(50), last_name varchar(50), phone_number varchar(50), hire_date date, job_id
varchar(50), salary decimal(12,2), manager_id int, department_id int);

alter table employee

-> AUTO_INCREMENT = 100;

MariaDB [college]> desc employeedate;

insert into employeedate(first_name, last_name, phone_number, hire_date, job_id, salary, manager_id, department_id) values('steven','king','515.123.4567','1987-06- 17','ad_pres',24000.00,0,90);

insert into employeedate(first_name, last_name, phone_number, hire_date, job_id, salary, manager_id, department_id) values ('neeena','Kochhar','515.123.4568', '1987-06- 18','AD_VP',17000.00,100,90);

insert into employeedate(first_name, last_name, phone_number, hire_date, job_id, salary, manager_id, department_id) values ('Lex','De Haan','515.123.4569','1987-06- 19','AD_VP',17000.00,100,90),('Alexander','Hunold','590.423.4567','1987-06- 20','IT_PROG',9000.00,102,60),('Bruce','Ernst','590.423.4568','1987-06- 21','IT_PROG',6000.00,103 ,60 ),('David','Austin','590.423.4569','1987-06- 22','IT_PROG',4800.00,103,60),('Valli','Pataballa','590.423.4560','1987-06-23',
'IT_PROG',4800.00,103,60),('Diana','Lorentz','590.423.5567','1987-06- 24','IT_PROG',4200.00,103,,60),('Nancy','Greenberg','515.124.4569','1987-06- 25','FI_MGR',12000.00,101, 100),('Daniel','Faviet','515.124.4169','1987-06-26','FI_ACCOUNT', 9000.00, 108 , 100),('John', 'Chen','515.124.4269','1987-06- 27','FI_ACCOUNT',8200.00,108,100),('Ismael','Sciarra','515.124.4369','1987-06- 28','FI_ACCOUNT', 7700.00, 108,100),('Jose Manuel','Urman','515.124.4469','1987-06- 29','FI_ACCOUNT',7800.00, 108, 100),('Luis','Popp','515.124.4567','1987-06- 30','FI_ACCOUNT',6900.00,108,100),('Den','Raphaely','515.127.4561','1987-07- 01','PU_MAN',11000.00,100,30),('Alexander', 'Khoo', '515.127.4562','1987-07-
02','PU_CLERK',3100.00, 114, 30),('Shelli',' Baida','515.127.4563', '1987-07-03','PU_CLERK', 2900.00,114,30),('Sigal', 'Tobias', '515.127.4564','1987-07-04','PU_CLERK', 2800.00 , 114, 30),( 'Guy','Himuro',' 515.127.4565', '1987-07-05','PU_CLERK',2600.00, 114, 30),('Karen','Colmenares' ,'515.127.4566','1987-07-06','PU_CLERK',2500.00, 114, 30 ),('Matthew', 'Weiss','650.123.1234','1987-07-07','ST_MAN', 8000.00,100, 50);
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that
corresponds to your MariaDB server version for the right syntax to use near
'60),('Nancy','Greenberg','515.124.4569','1987-06-25','FI_MGR',12000.00,101, 1...' at line 1
MariaDB [college]> insert into employeedate(first_name, last_name, phone_number, hire_date, job_id, salary, manager_id, department_id) values ('Lex','De
Haan','515.123.4569','1987-06- 19','AD_VP',17000.00,100,90),('Alexander','Hunold','590.423.4567','1987-06- 20','IT_PROG',9000.00,102,60),('Bruce','Ernst','590.423.4568','1987-06- 21','IT_PROG',6000.00,103 ,60 ),('David','Austin','590.423.4569','1987-06- 22','IT_PROG',4800.00,103,60),('Valli','Pataballa','590.423.4560','1987-06-23',
'IT_PROG',4800.00,103,60),('Diana','Lorentz','590.423.5567','1987-06- 24','IT_PROG',4200.00,103,,60),('Nancy','Greenberg','515.124.4569','1987-06- 25','FI_MGR',12000.00,101,100),('Daniel','Faviet','515.124.4169','1987-06-26','FI_ACCOUNT', 9000.00, 108 , 100),('John', 'Chen','515.124.4269','1987-06- 27','FI_ACCOUNT',8200.00,108,100),('Ismael','Sciarra','515.124.4369','1987-06- 28','FI_ACCOUNT', 7700.00, 108,100),('Jose Manuel','Urman','515.124.4469','1987-06- 29','FI_ACCOUNT',7800.00, 108, 100),('Luis','Popp','515.124.4567','1987-06- 30','FI_ACCOUNT',6900.00,108,100),('Den','Raphaely','515.127.4561','1987-07- 01','PU_MAN',11000.00,100,30),('Alexander', 'Khoo', '515.127.4562','1987-07- 02','PU_CLERK',3100.00, 114, 30),('Shelli',' Baida','515.127.4563', '1987-07-03','PU_CLERK', 2900.00,114,30),('Sigal', 'Tobias', '515.127.4564','1987-07-04','PU_CLERK', 2800.00 , 114, 30),( 'Guy','Himuro',' 515.127.4565', '1987-07-05','PU_CLERK',2600.00, 114, 30),('Karen','Colmenares' ,'515.127.4566','1987-07-06','PU_CLERK',2500.00, 114, 30 ),('Matthew', 'Weiss','650.123.1234','1987-07-07','ST_MAN', 8000.00,100, 50);
ERROR 1064 (42000): You have an error in your SQL syntax; check the manual that
corresponds to your MariaDB server version for the right syntax to use near
'60),('Nancy','Greenberg','515.124.4569','1987-06-25','FI_MGR',12000.00,101,10...' at line 1
MariaDB [college]> insert into employeedate(first_name, last_name, phone_number, hire_date, job_id, salary, manager_id, department_id) values ('Lex','De
Haan','515.123.4569','1987-06- 19','AD_VP',17000.00,100,90),('Alexander','Hunold','590.423.4567','1987-06- 20','IT_PROG',9000.00,102,60),('Bruce','Ernst','590.423.4568','1987-06- 21','IT_PROG',6000.00,103 ,60 ),('David','Austin','590.423.4569','1987-06- 22','IT_PROG',4800.00,103,60),('Valli','Pataballa','590.423.4560','1987-06-23',
'IT_PROG',4800.00,103,60),('Diana','Lorentz','590.423.5567','1987-06- 24','IT_PROG',4200.00,103,60),('Nancy','Greenberg','515.124.4569','1987-06- 25','FI_MGR',12000.00,101,100),('Daniel','Faviet','515.124.4169','1987-06-26','FI_ACCOUNT', 9000.00, 108 , 100),('John', 'Chen','515.124.4269','1987-06- 27','FI_ACCOUNT',8200.00,108,100),('Ismael','Sciarra','515.124.4369','1987-06- 28','FI_ACCOUNT', 7700.00, 108,100),('Jose Manuel','Urman','515.124.4469','1987-06- 29','FI_ACCOUNT',7800.00, 108, 100),('Luis','Popp','515.124.4567','1987-06- 30','FI_ACCOUNT',6900.00,108,100),('Den','Raphaely','515.127.4561','1987-07- 01','PU_MAN',11000.00,100,30),('Alexander', 'Khoo', '515.127.4562','1987-07- 02','PU_CLERK',3100.00, 114, 30),('Shelli',' Baida','515.127.4563', '1987-07-03','PU_CLERK', 2900.00,114,30),('Sigal', 'Tobias', '515.127.4564','1987-07-04','PU_CLERK', 2800.00 , 114, 30),( 'Guy','Himuro',' 515.127.4565', '1987-07-05','PU_CLERK',2600.00, 114,
30),('Karen','Colmenares' ,'515.127.4566','1987-07-06','PU_CLERK',2500.00, 114, 30 ),('Matthew', 'Weiss','650.123.1234','1987-07-07','ST_MAN', 8000.00,100, 50);


Q.1) Write a query to display the names (first_name, last_name) using alias name "First
Name", "Last Name".

Query: select first_name as First Name , last_name as Last Name from employeedata;

Q.2)Write a query to get unique department ID from employee table.

Query: select distinct(department_id) from eployeedata;

Q.3)Write a query to get all employee details from the employee table order by first name, descending.

Query: select * from employeedata order by first_name desc;

Q.4)Write a query to get the employee ID, names (first_name, last_name), salary in
ascending order of salary.

Query: select employee_id, concat(first_name, ' ',last_name) as Name, salary from employeedata order by salary;

Q.5)Write a query to get the maximum and minimum salary from employees table.

Query: select Max(salary) as Max_Salary, min(salary) as Min_Salary from employeedata;

Q.6)Write a query to get the first 3 characters of first name from employees table.

Query: select substring(first_name,1,3) as 'First_3_char'from employeedata;

Q.7)Write a query to display the name (first_name, last_name) and department ID of all
employees in departments 30 or 90 in ascending order.

Query:select first_name, last_name from employeedata where department_id in(30,90) order by department_id;


like operator
------------- 
Q.8)Write a query to display the last name of employees having 'e' as the third character.

Query: select last_name from employeedata where last_name like '__e%';


sub queries
----------- 
Q.9)Write a query to find the name (first_name, last_name) and the salary of the employees
who have a higher salary than the employee whose last_name= ‘Weiss’.

Query: select first_name, last_name, salary from employeedata where salary > (select salary from employeedata where last_name= 'Weiss');

Q.10)Write a query to find the name (first_name, last_name) of the employees who are
managers.

Query: select distinct m.first_name as First_Name, m.last_name as Last_name from employeedata e join employeedata m on e.manager_id= m.employee_id;



Date functions
---------------- 
Q.11)Write a query to get the firstname, lastname who joined in the month of June.

Query: select first_name, last_name, hire_date from employeedata where month(hire_date)= 6;


Joins 
===== 
Q.12) Question on self join

emp1: 
-----
id  name  manager_id
---------------------------
1  Harry   2
2  Mac     3
3  Rox     Null
4  Shree   2

o/p

employee_name manager_name
------------------------------
Harry        Mac
Mac          Rox
Shree        Mac

Query: select e.name as employee_name, m.name as manager_name from emp1 e join emp1 m on m.id= e.manager_id;


