## To create table
```bash
CREATE TABLE "Employee" (
	"Id"	INTEGER UNIQUE,
	"Name"	TEXT NOT NULL,
	"Salary"	INTEGER NOT NULL,
	"Age"	INTEGER NOT NULL,
	"Role"	TEXT NOT NULL,
	"Address"	TEXT NOT NULL,
	"Phone"	INTEGER NOT NULL,
	PRIMARY KEY("Id" AUTOINCREMENT)
);
```

## Add employee to the table

```bash
INSERT INTO Employee (Name, Salary, Age, Role, Address, Phone)
VALUES ('Yashu', 2000, 19, 'Manager', 'Balaji Banglows', 9638547575);
```

## Add multiple employee data to the table

```bash
INSERT INTO Employee (Name, Salary, Age, Role, Address, Phone)
 VALUES ('Hiren', 300, 19, 'Peune', 'Paravat Patiya', 1234567891);
```

## Retrive all data from the table
```bash
SELECT * FROM Employee;
```
## Find employees with a particular role

```bash
SELECT * FROM Employee WHERE Role = 'Peune'
```

## Search for employees with names containing "Sa"

```bash
SELECT * FROM Employee WHERE Name LIKE 'yA%'
```

## Find employees older than 30 and earning more than Rs.40000

```bash
SELECT * FROM Employee WHERE Age <  22 AND Salary < 1000
```

## Change the salary of an employee with ID

```bash
UPDATE Employee  SET Salary = 5000 WHERE Id = 20
```

## Update the address for employees in the 'Flutter Developer' role

```bash
 UPDATE Employee SET Address = 'Om Nagar' WHERE Role = 'Manager'
```

## Remove an employee with ID 2

```bash
DELETE FROM Employee WHERE Id = 20
```

## Delete all employees under 18 (assuming it's not a valid age)

```bash
DELETE FROM Employee WHERE Age < 20
```

## Table
<img src="https://github.com/user-attachments/assets/91281c88-40f7-4066-b207-d9844a009f33">
