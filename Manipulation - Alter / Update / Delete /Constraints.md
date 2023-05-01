## Alter table ##

The ALTER statement is used to append a new column to an existing table. 

Below is the query to add a new column 'Department' and set a default value, to the existing table student.


```c
ALTER TABLE student
ADD COLUMN Department TEXT default NULL;
```


## Update table ##
The UPDATE statement is used to edit a row or multiple rows in a table. 

```c
UPDATE student
 SET Age = 6
 WHERE student_id = 23;   
 
 Select * from employee;
 
 The 'WHERE' condition can be applied for any column.
 ```
 
 
## Delete From ##
 
 The DELETE FROM statement is used to remove one or multiple rows from a table.
 
 Below is the query to delete all rows in the student table with student_id - 08
 
 ```c
 DELETE FROM  student
 WHERE student_id = 08;
 ```
 
 
 ## Constraints ##

Constraints provide details about the usage of a column and are applied after specifying the column's data type. 
They enable the database to reject any inserted data that violates a particular constraint. 

```c
CREATE TABLE  student(
 student_id INTEGER PRIMARY KEY,
 student_Name TEXT UNIQUE,
 Department TEXT NOT NULL); 
 ```
 
**PRIMARY KEY**
can be utilized to uniquely identify a row in a table.
When attempting to insert a row with the same value as an existing row in the table, a constraint violation will occur, preventing the insertion of the new row.


**UNIQUE**
columns contain distinct values for each row, similar to "PRIMARY KEY" columns, but unlike primary key columns, a table can have multiple unique columns.


**NOT NULL**
columns must have a value assigned to them. 


When attempting to insert a row without providing a value for a "NOT NULL" column, a constraint violation will occur, preventing the insertion of the new row.

 
 
 Example-:
 
 ```c
 CREATE TABLE employee(
 employee_id INTEGER PRIMARY KEY,
 employee_Name TEXT UNIQUE,
 Department TEXT NOT NULL); 
 
 Select * from employee;
 ```
 
 
 
 
 
 
 
 
 

