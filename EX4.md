# Ex. No: 4 Creating Procedures using PL/SQL

### AIM: To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:
i) Creating table:
```sql
 create table employee(empid number, empname varchar(10), dept varchar(10), salary number);
```
ii) Creating procedure:
```sql
create or replace procedure employee_data as
    begin
    insert into employee(empid,empname,dept,salary) values (1,'Sita','HR',70000);
    insert into employee(empid,empname,dept,salary) values (2,'Anjali','MD',95000);
    insert into employee(empid,empname,dept,salary) values (3,'Chandhini','Finance',80000);
    commit;
    end;
    /
 begin
    employee_data;
    end;
    /
```
### Output:
![image](https://github.com/DHARINIPV/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/119400845/2c4fabb2-8426-496d-820d-1994cbd32f48)

![image](https://github.com/DHARINIPV/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/119400845/bfacd48b-71d7-4409-a574-b48f11fbbace)

### Result:
Hence the procedure using pl/sql is created successfully.
