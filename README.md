# SQLite_Database

# Employee Database Management System

#### An Employee Database Management System with SQLite is a software tool that uses SQLite to manage and store employee records, enabling CRUD (Create, Read, Update, Delete) operations on employee data. It is designed for efficient data management with minimal setup, suitable for small to medium-sized organizations.

<h1 align="left"></h1>

<h2 align="center"> Create a DBMS for employees </h2>

```Field names: Id, Name, Role, Salary, Age, Adress, Phone.```

<h1 align="left"></h1>

## Syntax

```
CREATE TABLE books (
    Name TEXT,
    Role TEXT,
    Salary INT,
    Age INT,
    Adress TEXT,
    Phone INT,
);
```

<h1 align="left"></h1>
<div align="center">
  <img width="600"  src="https://github.com/user-attachments/assets/f91b7d6e-c2ba-4efa-a55b-9cb1f6f5c2be" />
</div>

<h1 align="left"></h1>
<h2 align="center"> Add a new employee with all the details </h2>

```Field names: Name, Role, Salary, Age, Adress, Phone.```

<h1 align="left"></h1>

## Syntax

```
INSERT INTO employee (Name,Role,Salary,Age,Adress,Phone) VALUES ('Hiren','CEO','1000000000',19,'19,Laxmi Park soc.,Godadara,
Surat',9054165198);
```

<h1 align="left"></h1>
<div align="center">
  <img width="600"  src="https://github.com/user-attachments/assets/d701167f-8139-4f31-8f63-8847162f6f25" />
</div>
<h1 align="left"></h1>
<div align="center">
  <img height="600"  src="https://github.com/user-attachments/assets/1665ef5f-b3a1-4074-9228-90a0ef79c5ef" />
</div>


<h1 align="left"></h1>
<h2 align="center"> Add multiple employees with selective data </h2>

```Field names: Name, Role, Salary, Age, Adress, Phone.```

<h1 align="left"></h1>

## Syntax

```
INSERT INTO employee (Name,Role,Salary,Age,Adress,Phone) VALUES ('Naresh','Chairman','2000000000',22,'Dindoli',2992321932);
INSERT INTO employee (Name,Role,Salary,Age,Adress,Phone) VALUES ('Sanju','Director','210000000',19,'Udhna',4701259318);
INSERT INTO employee (Name,Role,Salary,Age,Adress,Phone) VALUES ('Yanshu','Director','2200000000',20,'Omnagar',3934235822);
```

<h1 align="left"></h1>
<div align="center">
  <img width="600"  src="https://github.com/user-attachments/assets/f5588e03-74af-4710-bf9f-8aa397d648f9" />
</div>
<h1 align="left"></h1>
<div align="center">
  <img height="600"  src="https://github.com/user-attachments/assets/8c49aeec-809c-47ab-9043-0fd7cc9da5a7" />
</div>

<h1 align="left"></h1>
<h2 align="center"> Retrieve all employee information </h2>

```Field names: Name, Role, Salary, Age, Adress, Phone.```

<h1 align="left"></h1>

## Syntax

```
SELECT * FROM employee
```

<h1 align="left"></h1>
<div align="center">
  <img width="600"  src="https://github.com/user-attachments/assets/c2fbcfa7-eabf-4992-8fbd-1484c957d008" />
</div>



<h1 align="left"></h1>
<h2 align="center"> Get specific columns for all employees (e.g., Name, Id) </h2>

## Syntax

```
SELECT * FROM employee WHERE Id = 1 AND Name = 'Hiren';
```

<h1 align="left"></h1>
<div align="center">
  <img width="600"  src="https://github.com/user-attachments/assets/2e280932-7956-496b-9777-ea2561e6cb98" />
</div>

<h1 align="left"></h1>
<h2 align="center"> Find employees with a particular role (e.g., Manager) </h2>

## Syntax

```
SELECT * FROM employee WHERE Role = 'Director';
```

<h1 align="left"></h1>
<div align="center">
  <img width="600"  src="https://github.com/user-attachments/assets/f720b03b-677c-4f2b-9735-3da0be45a1df" />
</div>

<h1 align="left"></h1>
<h2 align="center"> Search for employees with names containing "An" (case-insensitive) </h2>

## Syntax

```
SELECT * FROM employee WHERE Name LIKE 'NA%';
```

<h1 align="left"></h1>
<div align="center">
  <img width="600"  src="https://github.com/user-attachments/assets/3ad023cf-8c99-4b77-8b7d-d5153b3ff522" />
</div>

<h1 align="left"></h1>
<h2 align="center"> Find employees older than 20 and earning more than $10,00,000 </h2>

## Syntax

```
SELECT * FROM employee WHERE Age > 20 AND Salary > 1000000;
```

<h1 align="left"></h1>
<div align="center">
  <img width="600"  src="https://github.com/user-attachments/assets/a548100f-4bd9-4398-8a37-768313c93d6a" />
</div>

<h1 align="left"></h1>
<h2 align="center"> Change the salary of an employee with ID 3 </h2>

## Syntax

```
UPDATE employee SET Salary = 2100000000 WHERE Id = 3;
```

<h1 align="left"></h1>
<div align="center">
<img width="600"  src="https://github.com/user-attachments/assets/cf4dd7f7-d24e-419b-b2f5-b7cea58ebcec" />
</div>
<h1 align="left"></h1>
<div align="center">
<img width="600"  src="https://github.com/user-attachments/assets/1b8303fa-7f0e-42de-99c0-8b729f02ab0f" />
</div>


<h1 align="left"></h1>
<h2 align="center"> Update the address for employees in the 'Chairman' role </h2>

## Syntax

```
UPDATE employee SET Adress = 'Delvada' WHERE Role = 'Chairman';
```

<h1 align="left"></h1>
<div align="center">
<img width="600"  src="https://github.com/user-attachments/assets/05e7b9ef-65f8-496f-81f1-182465d42aef" />
</div>
<h1 align="left"></h1>
<div align="center">
<img width="600"  src="https://github.com/user-attachments/assets/37975027-4fbb-47d5-acf8-e65661a470b5" />
</div>


<h1 align="left"></h1>
<h2 align="center"> Remove an employee with ID 1 </h2>

## Syntax

```
DELETE FROM employee WHERE Id = 1;
```

<h1 align="left"></h1>
<div align="center">
<img width="600"  src="https://github.com/user-attachments/assets/4c85fe1e-797f-4d18-a285-81f9e00e0952" />
</div>
<h1 align="left"></h1>
<div align="center">
<img width="600"  src="https://github.com/user-attachments/assets/1cf73a32-8577-42a9-becb-9bd94dbfaf07" />
</div>

<h1 align="left"></h1>
<h2 align="center"> Delete all employees under 20 (assuming it's not a valid age) </h2>

## Syntax

```
DELETE FROM employee WHERE Age < 20;
```

<h1 align="left"></h1>
<div align="center">
<img width="600"  src="https://github.com/user-attachments/assets/2a6ac5e5-c78f-46cb-be8c-c8f62ef2244b" />
</div>
<h1 align="left"></h1>
<div align="center">
<img width="600"  src="https://github.com/user-attachments/assets/dda15557-0aff-4b1a-96a3-043a40d3111c" />
</div>
