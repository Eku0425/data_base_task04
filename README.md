# data_base_task04

## Field names: id, name, role, salary, age, address, phone.
CREATE TABLE "employee" (

	"id"	INTEGER,
	"name"	TEXT NOT NULL,
	"role"	TEXT NOT NULL,
	"salary"	INTEGER,
	"age"	INTEGER NOT NULL,
	"address"	TEXT,
	"phone"	INTEGER NOT NULL,
	PRIMARY KEY("id" AUTOINCREMENT)

);
 
## Add a new employee with all the details
INSERT INTO employee(name,role,salary,age,address,phone) VALUES('Ekta','Flutter Developer',100000,20,'201,Kodiyar  Soc,surat',2538172972);
Insert emloyees data
Add multiple employees with selective data:
INSERT INTO employee(name,role,salary,age,address,phone) VALUES ('Ekta','Flutter Developer',100000,20,'201,Khodiyar Soc,surat',2538172972);
INSERT INTO employee(name,role,salary,age,address,phone) VALUES ('Abhi','Flutter Developer',50000,21,'6501,shanti nagar , surat' , 361728134);
INSERT INTO employee(name,role,salary,age,address,phone) VALUES ('Netra','FullStack Develoer',60000,25,'167,chikuvadi pandesara',1357278342);
INSERT INTO employee(name,role,salary,age,address,phone) VALUES ('kuldeep','Ui-Ux Designer',80000,25,'100,dindoli,surat',1362738274);
INSERT INTO employee(name,role,salary,age,address,phone) VALUES ('trusha','Ui-Ux Designer',90000,23,'502,krishna park ,baroda ',136772883);
 
## Read data
Retrieve all employee information:
  SELECT * FROM   employee;
Get specific columns for all employees (e.g., name, salary)
SELECT  name,salary FROM employee WHERE name =name;
Find employees with a particular role (e.g., Manager):
SELECT  name,role FROM employee WHERE role ='Flutter Devloper';
Search for employees with names containing "An" (case-insensitive):
SELECT  name FROM employee WHERE name LIKE 'S%';
Find employees older than 20 and earning more than 25,000:
SELECT * FROM employee WHERE  (salary>25000)AND age>20;
Change the salary of an employee with ID 1:
UPDATE employee
SET salary = 50000
WHERE id =11
Update the address for employees in the 'Flutter Devloper' role:
UPDATE employee SET address = '201,dhruv Park Soc,surat' WHERE role  = 'Flutter Devloper';
Remove an employee with ID 101:
DELETE FROM employee WHERE id = 13;
.
