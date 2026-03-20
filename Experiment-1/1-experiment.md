# Experiment 1

## Aim

To perform basic SQL operations such as creating a table from an existing table, deleting records, updating values, altering table structure, and dropping a table.

---

## Theory

SQL (Structured Query Language) is used to manage and manipulate relational databases. It provides commands to create, modify, and delete data efficiently.

In this experiment:

* A new table is created using data from an existing table
* Specific records are deleted based on a condition
* Existing data is updated
* The table structure is modified
* The table is deleted after operations

These operations help in understanding how real-world databases are managed and maintained.

---

## Queries

### 1. Create Employee_master table with data

sql
CREATE TABLE Employee_master AS
SELECT * FROM EMPLOYEE;


---

### 2. Delete records where DeptNo = 10

sql
DELETE FROM Employee_master
WHERE DEPTNO = 10;


---

### 3. Update 10% salary for DeptNo = 20

sql
UPDATE Employee_master
SET SAL = SAL + (SAL * 0.10)
WHERE DEPTNO = 20;


---

### 4. Alter SAL column size

sql
ALTER TABLE Employee_master
MODIFY SAL NUMBER(10,2);


---

### 5. Drop Employee_master table

sql
DROP TABLE Employee_master;


---

## Result

The required SQL operations were performed successfully on the Employee_master table.
