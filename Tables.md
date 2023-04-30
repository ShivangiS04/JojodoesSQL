
## Create table

Using a CREATE statement in SQL enables the creation of a new table in the database. 
This statement can be used whenever a new table needs to be created, starting with a blank slate. 

```c

CREATE TABLE student (
   Student_id INT,
   Student_Name  TEXT,
   Department  TEXT
); 
```

## Insert table 

Rows are added into a table using the **INSERT** statement. 


```c
/* Write a query to insert the below mentioned employee details to the table 'employee' */
INSERT INTO employee(employee_id,employee_Name,Department)
 VALUES (04,'Marcus Garcia','Product'),
        (05,'Mike Tyson','HR');
```

