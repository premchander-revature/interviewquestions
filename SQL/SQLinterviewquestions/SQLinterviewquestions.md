1. Comparing the given two tables, fetch the values from the table Sample_a that are not common in table Sample_b, without using the NOT keyword.

  Two tables are created as follows:

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

```sql
create table Sample_a(ID numeric);

create table Sample_b(ID numeric);

insert into Sample_a(ID) values
(10),
(20),
(30),
(40),
(50);

insert into Sample_b(ID) values
(10),
(30),
(50);

```


<details>
<summary>Show Answer</summary>
<blockquote>

```sql

select * from Sample_a
except
select * from Sample_b;

```

</blockquote>
</details>

---

2.Debug the given SQL query:

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

```sql
SELECT id, name
FROM students
WHERE grades =
             (SELECT MAX(grades)
              FROM students
              GROUP BY subject_id);

```
<details>
<summary> Show Answer </summary>
<blockquote>

```sql
        SELECT MARKS, COUNT (DISTINCT STUDENT_ID) 
        FROM STUDENT 
        GROUP BY MARKS 
        HAVING MARKS > (SELECT AVG(MARKS) 
                   FROM STUDENT 
                   WHERE ADDRESS = ’NOIDA’ );

```

  </blockquote>
<details>
<summary> Explanation </summary>
<blockquote>  

    In the above query, we used GROUP BY MARKS. It clusters the rows with same Marks and we also use SELECT MARKS, COUNT(DISTINCT STUDENT_ID) which prints the marks of each cluster and the count of the rows of respective clusters. 

</blockquote>

</details>
</details>

---


3.Debug the given SQL query:

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

```sql
SELECT Id, name, YEAR(BillingDate) AS Year
FROM Records
WHERE Year >= 2010

```
<details>
<summary> Show Answer </summary>

<blockquote>

```sql

    SELECT Id, name, YEAR(BillingDate) AS Year
    FROM Records
    WHERE Year(BillingDate) >= 2010;
```

  </blockquote>
  
  <details>
<summary> Explanation </summary>
  
<blockquote>

    The expression BillingYear in the WHERE clause is invalid. Even though it is defined as an alias in the SELECT phrase, which appears before the WHERE phrase, the logical processing order of the phrases of the statement is different from the written order.

</blockquote>
</details>
</details>

---

4.Which of the following SQL query tracks the names of the sailors who have reserved atleast one boat?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

```sql

a.SELECT DISTINCT s.name FROM sailors , reserves WHERE s.sid = r.sid;

b.SELECT s.sname FROM sailors s ,reservers r WHERE s.sid = r.sid;

c.SELECT DISTINCT s.name FROM sailors s, reserves r WHERE s.sid = r.sid;

d.None of these

```
<details>
<summary> Show Answer </summary>
<blockquote>

C.SELECT DISTINCT s.name FROM sailors s, reserves r WHERE s.sid = r.sid;

</blockquote>

</details>

---

5.After the completion of a transaction in SQL, it must be executed to save all the operations performed in the transaction. Which command is used for this?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)


 a. REVOKE

 b. COMMIT

 c. ROLLBACK

 d. SAVE
<details>

<summary> Show Answer </summary>
<blockquote>

b) COMMIT

</blockquote>

  <details>
<summary> Explanation </summary>
<blockquote>

 The COMMIT command must be executed to save all the operations performed in the transaction.

</blockquote>
  </details>
</details>

---

6.Which of the following SQL statement is valid?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
```sql

a.SELECT \_ FROM Employees WHERE Gender = 'F';

b.SELECT \_ FROM Employees;

c.SELECT Gender= 'M' FROM Employees;

d.SELECT Gender FROM Employees WHERE Last_Name = 'Gowda';

```

<details>
<summary>Show Answer</summary>
<blockquote>

```sql

 d.SELECT Gender FROM Employees WHERE Last_Name = 'Gowda';

```
</blockquote>

<details>
<summary>Explanation</summary>
<blockquote>

The Statement in Option d is used to Select the Gender data from the table with a where condition stating that the last name should be "Gowda" which is a valid query.
</blockquote>
</details>
</details>

---

7.Write a SQL query for the below tableto get the employee details using the last name?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)


|Table: Employees                                            |
|First_Name | Last_Name | Birth_Date | Gender | Joining_Date |
|-----------|-----------|------------|--------|--------------|
|Ajay       | Kumar     | Mar-15-1970| M      | Apr-05-2017  |
| David     | Richard   | Feb-17-1985| M      | Mar-05-2017  |
|Junaid     | M         | Sep-28-1987| M      | Mar-09-2016  |
|Janvi      | Gowda     | Oct-22-1993| F      | Apr-09-2015  |
|Shobika    | Kumar     | Aug-22-1996| F      | Apr-15-2014  |

```sql

a. SELECT \* FROM Employees WHERE Gender = 'F';

b. SELECT \* WHERE Gender = 'M' FROM Employees;

c. SELECT Gender= 'M' FROM Employees;

d. SELECT Gender FROM Employees WHERE Last_Name = 'Kumar';

```

<details>

<summary> show answer </summary>

<blockquote>

d) SELECT Gender FROM Employees WHERE Last_Name = 'Kumar';

</blockquote>

<details>

<summary>Explanation</summary>

<blockquote>

By using SELECT key in addition to WHERE clause be used for Last_Name

</blockquote>

</details>
</details>

---

8.Which of the following statement is true?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)


a.With the DDL commands, any structural changes can be made to the table, including creation, deletion, and alteration.

b.With the DML commands, any structural changes can be made to the table, including creation, deletion, and alteration.

c.With the DCL commands, any structural changes can be made to the table, including creation, deletion, and alteration.

d.With the TCL commands, any structural changes can be made to the table, including creation, deletion, and alteration

<details>
<summary>Show Answer</summary>
<blockquote>

a) With the DDL commands, any structural changes can be made to the table, including creation, deletion, and alteration.

</blockquote>

<details>
<summary>Explanation</summary>
<blockquote>

Data definition language (DDL) refers to the set of SQL commands that can create and manipulate the structures of a database. DDL statements are used to create, change, and remove objects including indexes, triggers, tables, and views.

</blockquote>
</details>
</details>

---

9.Which of the following statement is used to get all datas whose name starts with p from a student table?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.SELECT \* FROM student WHERE name LIKE '%p%';

b.SELECT \* FROM student WHERE name LIKE '\_p%';

c.SELECT \* FROM student WHERE name LIKE 'p%';

d.SELECT \* FROM student WHERE name LIKE '%p';

<details>
<summary>Show Answer</summary>
<blockquote>

c. SELECT \* FROM student WHERE name LIKE 'p%';

</blockquote>

<details>
<summary>Explanation</summary>
<blockquote>

- The '%' symbol indicates zero or more characters next to where it will be used.
- The \_ symbol is used to match exactly one character. Therefore, option C is the correct choice.
</blockquote>
</details>
</details>

---

10. Consider an Employee table that has 10 Records and it has a non - NULL SALARY column which is also UNIQUE. Based on these, predict the output for the given SQL statement.

```sql
SELECT COUNT(*) FROM Employee WHERE SALARY > ANY (SELECT SALARY FROM EMPLOYEE);

```
a.10

b.5

c.9

d.0

<details>
<summary> Show Answer </summary>
<blockquote>

b.5

</blockquote>

<details>
<summary>Explanation</summary>
<blockquote>

Each non-NULL value in the SALARY column of the employee table's 10 records is distinct, i.e. different. As a result, out of those ten records, one must be a minimum and cannot exceed any of the nine values in the pay column. So, nine times will the condition WHERE SALARY > ANY (SELECT SALARY FROM employee) be true. The COUNT(*) returns 9.
</blockquote>
</details>
</details>

---

11.What are the functional differences of Drop and Truncate?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- The DROP command is used to delete all the data in a table or database, including any indexes and data. In contrast, the TRUNCATE command is used to remove all of the table's rows.

</blockquote>
</details>

------

12.How to quickly retrieve records from a table. Give an explanation.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- The database search engine can speed up data retrieval by using indexes, which are specialised lookup tables. 
- An index can be thought of as a pointer to information in a table.
- The index in the back of a book is nearly identical to an index in a database.

</blockquote>
</details>

------

13.What will happen if the statement's DEFAULT clause provision is deleted?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

Table will be created with no default value for CREATE_DATE column

</blockquote>
</details>

------

14.A table is created for a bank department. Which datatype is used to store an interval of days, hours, minutes and seconds in a column?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

INTERVAL YEAR TO MONTH

</blockquote>
</details>

------

15.What are the reliablities for table creation?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- It's not necessary to mention a table's size. Online table editing is possible. 
- To create the table's structure, each column needs attributes such as data kinds and precision.

</blockquote>
</details>

---

16. What happens when a transaction function is issued against a DDL command?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- The transaction is committed and terminated
- The current transaction will be committed and stopped if a DDL statement is used. The current transaction will make permanent all database modifications. The DDL statement refers to this as an implicit commit.

</blockquote>
</details>

---


17.What is schema and what is its reliablity?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- A schema in a SQL database is a list of logical data structures. The schema, which shares the same name as the database manager, is owned by a database user.
- It consists of a group of database items related to a database.

</blockquote>
</details>

------

18.By using quoted Identifiers ' ', you could create tables. How would you reference those table?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

"table_name" 
- When a table is made using a sub-query, a LONG column is not replicated.
- The LONG column is not copied when a table is created using the CTAS (CREATE TABLE AS SELECT) method.

</blockquote>
</details>

------

19.What is accurate regarding a table obtained by a sub-query? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- When a table is made using a sub-query, a LONG column is not replicated.
- The LONG column is not copied when a table is created using the CTAS (CREATE TABLE AS SELECT) method.

</blockquote>
</details>

------

20.How would you determine the referenced data when you delete the parent record?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

The ON DELETE clause is a foreign key's clause.
There are two options:
- ON DELETE SET NULL: When the parent record is deleted, all of the child records' referenced columns will be set to NULL.
- ON DELETE SET CASCADE: All of the child records will also be removed when the parent record is deleted.

</blockquote>
</details>

------

21.How do we copy the existing table without affecting the real table and use the same for the development purposes?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Show Answer</b> </summary>

```sql
CREATE TABLE table_name AS (SELECT select_query);
```

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- You can specify the table_name for your new table, as well need to use a `SELECT` query.
- If you need to copied all the records from the existing table mentioning `SELECT * FROM` to new table.
- It also refered as `CTAS`(`CREATE TABLE AS SELECT`)

</blockquote>

</details>
</details>

------

22.Write a sample query for the annual function in the office and how do we create an event?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary> <b>Show Answer</b> </summary>

```sql
CREATE EVENT event_name 
ON SCHEDULE AT CURRENT_TIMESTAMP + INTERVAL 1 HOUR 
DO 
UPDATE myschema.mytable SET mycol = mycol +1 ;
```

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- In the above query, `CREATE EVENT` keyword along with event name is used to identifies the event name in database schema.
- `ON SCHEDULE` clause is used to determine how the event executes.
- `DO` clause is the sql statement for the execution.

</blockquote>

</details>
</details>

-------

23. Create a table for list of cities on weather monitoring that holds datas of latitude_north,longitude_west and temperature with NO duplicate ID fields.

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary> <b> Show Answer </b> </summary>

```sql
CREATE TABLE WEATHER_MONITOR (ID INT PRIMARY KEY, CITY VARCHAR(30), STATE VARCHAR(30), TEMP REAL, LATITUDE_N REAL, LONGITUDE_W REAL);
```
<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

Create a table along with a table name "WEATHER_MONITOR" contains fields such as ID with the datatype `INTEGER`, CITY with the datatype `VARCHAR`, STATE with the datatype `VARCHAR`, TEMPERATURE, LATITUDE_N, LONGITUDE_W with the datatype `REAL`.

</blockquote>

</details>
</details>

-------

24. Write a SQL query to get the below table displayed as output in undefined order.

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)


Table: WEATHER_MONITOR

|  ID |   CITY	    |   STATE      |   TEMP   |  LATITUDE_N   |LONGITUDE_W |
|-----|-------------|--------------|----------|---------------|----------- |
| 10  |  HOUSTON	|  	TEXAS      |   15.6   | 	 33       |     112    |
| 123 | LOS ANGELES	| CALIFORNIA   |   18.3   | 	 45       |     134    |



<details>
<summary><b> Show Answer </b></summary>

<blockquote>

``` sql
SELECT * FROM WEATHER_MONITOR;
```
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

By using `SELECT` Command following `*` along with the table name.

</details>
</details>

------


25.Write a SQl query to add a constraint to a EMPLOYEE table that restricts the addition of employees whose salary is less than 10000.

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)


<details>
<summary> <b> Show Answer </b> </summary>

```sql
ALTER TABLE employees ADD CONSTRAINT emp_salary CHECK (salary <10000)
```
<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

Using `ALTER` command adding the `CONSTRAINT` in emp_salary column checking the the condition less than 10000.

</blockquote>

</details>
</details>

-------



26. Which commands are used to manage transactions in the database?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Explanation</b></summary>

<blockquote>

Transaction Control Language commands are used to manage transactions in the database. These are used to manage the changes made by DML-statements. It also allows statements to be grouped together into logical transactions.

</blockquote>

</details>

---

27.Which command is used to temporarily save a transaction so that you can rollback to that point whenever necessary?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Explanation</b></summary>

<blockquote>

`SAVEPOINT` is the TCL Command which is used to temporarily save a transaction so that it can be rollbacked to that particular point when necessary.

</blockquote>

</details>

---

28.Which Command undoes all the changes done by the current transaction?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Explanation</b></summary>

<blockquote>

`ROLLBACK` is the command which undoes all the changes done by the current transaction.

</blockquote>

</details>

---

29.Which Command is used to Save a data in the table Permanently?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Explanation</b></summary>

<blockquote>

`COMMIT` is the TCL Command whis is used to permanently save a data in a table inside a database.

</blockquote>

</details>

---

30.How to reduce the Data redundancy in a database?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Explanation</b></summary>

<blockquote>

Normalization is the technique which is used to reduce the data Redundany in the databse in SQL.

</blockquote>

</details>

---

31.In What ways can we reduce the Data Redundancy in a Database?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Data Redundancy can be reduced by using different Normalization Techniques.

</blockquote>

<details>

<summary><b>Explanation</b></summary>

<blockquote>

Here is a list of Normalization Techniques in SQL:

- 1NF (First Normal Form)
- 2NF (Second Normal Form)
- 3NF (Third Normal Form)
- BCNF (Boyce-Codd Normal Form)
- 4NF (Fourth Normal Form)
- 5NF (Fifth Normal Form)
- 6NF (Sixth Normal Form)

</blockquote>

</details>

</details>

---

32.What are the Advantages of Reducing the Data Redundancy in a Database?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

- Data reliability

- Data consistency denotes that the data is always accurate and clear.

- Data stops being redundant.

- Non-redundant means that each user and every time has access to only the original copy of the data. There are no duplicates of the same information for various people.

</blockquote>

</details>

---

33.What are the Disadvantages of Reducing the Data Redundancy in a Database ?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

- The need for a skilled database designer exists.
- Difficult and expansive
- needs intricate database design

</blockquote>

</details>

---

34.In What ways can we increase the Data Redundancy in a Database?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

The Data Redundancy can be increased by using De-Normalization Techniques.

</blockquote>

<details>

<summary><b>Explanation</b></summary>

<blockquote>

The act of incorporating precomputed redundant data into a normalised relational database in order to enhance read performance is known as De-Normalization.

</details>

</details>

---

35.What do you Mean By Insert Anomaly in MYSQL?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

When we attempt to insert data into the database, but the data is incomplete or incorrectly placed into the target attributes, this is known as an insertion anomaly.

</blockquote>

</details>

---
  
36.Create a SQL query by using the `IN` Operator to determine whether the Employee's FirstName is present in the given table.
          Table_Name: Employee Table
|Emp_Id	|    First_Name  	  |      Last_Name    |      	Email_Id        |	Salary  | Dept_Id  |
|-------|-------------------|-------------------|-----------------------|---------|----------|
|  1	  |     John          |	     King         |	john.king@gmail.com   |	33000	  |    1     |
|  2	  |     James         |	     Bond         |	james@gmail.com       |	30000   |	   1     |
|  3	  |     Neena         |	    Kochhar       |   neena@gmail.com	    |   17000 |	   2     |
|  4	  |      Lex	        |       De Haan     |     lex@gmail.com	    |   15000	|    1     |
|  5	  |      Amit	        |        Patel      |	  amit@gmail.com	    |   18000	|    3     |
|  6	  |      Abdul	      |        Kalam      |    abdul@gmail.com	  |   25000	|    4     |

         Table_Name: Department Table

|  Dept_Id	|     Name    |
|-----------|-------------|
|     1     |    Finance  |
|     2     |     HR      |
|     3     |    Sales    |
|     4     |    Admin    |

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql
SELECT Emp_Id, First_Name, Last_Name, Salary
FROM Employee
WHERE Emp_Id IN (1, 3, 5, 6)
```
The above query will return records where Emp_Id is 1 or 3 or 5 or 6. 

The above query will display the following result.

|Emp_Id	|  First_Name |	Last_Name  |	Salary  |
|-------|-------------|------------|----------|
|  1    |	  John      |     King   |	33000   |
|  3    |	  Neena     |    Kochhar |  17000   |
|  5    |	  Amit      |    Patel   |	18000   |
|  6    |	  Abdul     |    Kalam   |	25000   |

</blockquote>

</details>

--------


37.Write a SQL query to find all the students, whose marks are greater than the average marks from the below table.
|   Stu_Id	|   Stu_Name	|  Marks   |  Average  |
|-----------|-------------|----------|-----------|
|     1     |	Akshaya     |	  78     |	  75     | 
|     2	    |   Divya	    |   65	   |    65     |
|     3     |	Bharathi	  |   77     |	  83     |

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql
SELECT  Stu_Name, Marks
FROM  Student_info
WHERE Marks > SELECT Average(Marks) FROM Student_info);
```

</blockquote>

</details>

--------

38.Debug the given SQL query?
  
  ```sql
SELECT Id, to_date(OrderDate,’YYYY’) AS OrderYear
FROM Order
WHERE OrderYear >= 2015;
```
  
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>


In the above query, OrderYear is an alias for to_date(OrderDate,’YYYY’) in SELECT clause.
When we are using OrderYear in WHERE clause, it is not available there.
The Following is the correct query:

```sql
SELECT Id, YEAR(OrderDate) AS OrderYear
FROM Order
WHERE YEAR(OrderDate) >= 2015;
```
</blockquote>

</details>

--------

39.Write a SQL query to find the first 10 employees from a list whose Employee ID's are odd numbers?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql
SELECT TOP 10 ID FROM Employee WHERE ID % 2 = 1;
```
</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

To find the Odd number Employee ID, we can use % function.

</blockquote>

</details>
</details>

--------

40.Write a SQL query to calculate the count of comma separated values for each names from the given Student table.

|   Student Name	|       Marks       |
|-----------------|-------------------|
|      Amit	      |    30,130,20,4    |
|    Sukruta	    |    100,20,30      |
|     Sonali	    |    140,10         |

Want to display output like :

|   Student Name	  |   Marks Count   |
|-------------------|-----------------|
|      Amit         |	    4           |
|     Sukruta       |	    3           | 
|     Sonali        |	    2           |

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql
SELECT Student_name, regexp_count (marks,’,’) + As “Marks Count” FROM Student;
```
</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

In real scenarios, lot of times developer needs to calculate the number of commas in the column then regexp_count function is used.

</blockquote>

</details>
</details>

------


41.How to create a Student1_table, which is an exact replica of Student_table?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql
CREATE Table Student_1 as SELECT * from Student;
```

</blockquote>

</details>

-----



42.Sailors(s_id, s_name, rating, age) with the following  data.



|   S_Id   |	S_Name	    |    Rating  |	Age    |
|----------|--------------|------------|---------|
|   22	   |    Avinash	  |      7	   |    45   |
|   29     |	  Raghu     |      1	   |    33   |
|   31	   |    Bharathi  |   	 8	   |    55   |
|   32	   |    Rohith	  |      8     |	  25   |
|   58	   |    Vishnu    |	    10     |	  17   |
|   64	   |    Sandhiya	|      7	   |    35   |
|   71	   |    Divya	    |     10	   |    16   |
|   74	   |    Yeshwini	|      9	   |    35   |
|   85	   |    Pooja	    |      3     |	  26   |
|   84	   |    Sangeetha | 	   3	   |    64   |
|   96	   |    Farin	    |      3	   |    17   |



For the Query,

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

```sql
SELECT  S.Rating, AVG(S.Age) AS average FROM Sailors s
WHERE S.Age>=18
GROUP BY S.Rating
HAVING 1<(SELECT COUNT(*) FROM Sailors S2 WHERE S.Rating = S.Rating)
```
The Number of rows returned is,
                   
a.	3 <br>
b.	4 <br>
c.	5 <br>
d.	6 <br>

<details>
<summary> Show Answer </summary>

<blockquote>

3

</blockquote>

</details>

-----

43.Which of the following do you need to consider when you create a table in SQL? <br>
a. Data types <br>
b. Primary Keys <br>
c. Default Values <br>
d. All of the above <br>


![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b> Show Answer </b></summary>

<blockquote>

Datatypes, Primary Key and Default values

</blockquote>

<details>
<summary> <b> Explanation </b></summary>

<blockquote>

Make sure when the column datatypes are the smallest required and to fit
the data comfortably.

</blockquote>

</details>
</details>

-----

 44.For any given User table, how could the name "Raju" in the "Name" column be changed to the name "Sanjana"?

<br>a. Update User Set Name = "Raju" INTO Name = "Sanjana"
<br>b. Modify Users SET Name = "Sanjana" WHERE Name = "Raju"
<br>c. Update Users SET Name = "Sanjana" WHERE Name = "Raju"
<br>d. Modify Users SET Name = "Raju" INTO Name = "Sanjana"


![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)


<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>

```sql
UPDATE Users SET Name = "Sanjana" WHERE Name = "Raju"
```
</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

The UPDATE command and WHERE clause are used together to change the name as asked in the question.

</blockquote>

</details>
</details>

------


45.What is the Output for the following table?

Let's take a Product table consisting of the following records and delete a single record from the given table below.

Table_Name: Product 
 

| Product_Id   |	Product_Name     |   Product_Price  |    Product_Quantity     |
|--------------|-----------------  |------------------|-------------------------|
|  P101	       |      Chips	       |           20     |         20              |
|  P102	       |      Chocolates   |           60	    |         40              |
|  P103	       |       Maggi	     |           75	    |          5              |
|  P104	       |       Biscuits	   |           80	    |         20              |
|  P105	       |      Namkeen	     |           40	    |         50              |


![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)


<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql
DELETE FROM Product WHERE Product_Id = P103 ; 
```
</blockquote>

| Product_Id   |	Product_Name     |   Product_Price	  |    Product_Quantity     |
|--------------|-------------------|--------------------|-------------------------|
|  P101	       |      Chips	       |           20       |         20              |
|  P102	       |      Chocolates   |           60	      |         40              |
|  P104	       |      Biscuits	   |           80	      |         20              |
|  P105	       |      Namkeen	     |           40	      |         50              |

<details>
<summary><b> Explanation </b><summary>

<blockquote>

To delete a particular row by using the delete command. The Syntax for deleting a row is ,
`DELETE` FROM Table_Name `WHERE` Condition ;

</blockquote>

</details>
</details>


-----

46.Write a SQL query to increase the income of all employees in Emp_Salary by 5% for the below employee table .

Table Name: Employees

           
         |  Emp_Id   |   Emp_Name   |   Emp_Salary  |
         |-----------|--------------|---------------|
         |   2010    |    Ankitha   |     28000     |
         |   2020    |    Kumar     |     23000     |
         |   2030    |    Diya      |     31000     |
         |   2040    |    Poornima  |     47000     |
         |   2050    |    Abinaya   |     20000     |


![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql
UPDATE Employees SET Emp_Salary = Emp_Salary+(Emp_Salary*5.0/100.0);
```

         |  Emp_Id   |   Emp_Name   |   Emp_Salary  |
         |-----------|--------------|---------------|
         |   2010    |	Ankitha	    |     29400     |
         |   2020    |  Kumar	      |     24150     |
         |   2030    |  Diya	      |     32550     |
         |   2040    |  Poornima    |     49350     |
         |   2050    |  Abinaya     |     21000     |

</blockquote>

<details>
<summary><b>Explanation</b></summary>

<blockquote>

Here `UPDATE` command is used for updating the salary by 5% and it is also can be used for only 5% alone it can be used for updating even 10% also.

</blockquote>

</details>
</details>

-----


47.The DDL, DCL, and DML language components that make up a database management system (DBMS).
Users and practitioners, two diverse groups of individuals, are both interested in them. Which of them do DBMS users often work with?

 a. DDL
 b. DML
 c. DDL and DCL
 d. DCL and DML

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)


<details>
<summary><b> Show Answer</b></summary>

<blockquote>

Data Manipulation Language

</blockquote>

<details>
<summary><b>Explanation</b></summary>

<blockquote>

Only the DBMS component for data manipulation language is of interest to users and practitioners.

</blockquote>

</details>
</details>

----

48.Write a query to create an empty table from an existing table?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Explanation </b></summary>

<blockquote>

An empty table is a table with same structure as the given table. But it does not contain records.
To create an empty table, we have to run a `SELECT` query so that no records are returned. But we can use the result of this query in `CREATE` statement to create an empty table.
To get no records in `SELECT` query, we can give a false condition like 1 > 2 in `WHERE` clause.
Query will be as follows:

```sql
CREATE TABLE Student_info  AS
SELECT * from Student
WHERE 1 > 2;
```
</blockquote>
</details>

----

49. For the given Employee table, where each employee has a DeptId, write a single SQL query to transfer personnel from DeptID 1 to DeptID 2 and vice versa.

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

Table: Employee

| ID  | NAME   | DEPT_ID |
| --- | ------ | ------- |
| 1   | JOHN   |    1    |
| 2   | GEORGE |    2    |
| 3   | JANE   |    1    |
| 4   | SMITH  |    2    |

<details>

<summary><b>Show Answer</b></summary>

We can use `CASE` statement here.

<blockquote>

```sql
UPDATE Employee SET DeptId =

            CASE DeptId

                        WHEN ‘1’ THEN ‘2’

                        WHEN ‘2’ THEN ‘1’

            ELSE DeptId END;

```

</blockquote>

</details>

---

50. Debug the below SQL query and predict the output for the list of workers who don't work for Dept. 1?

![Medium](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg>)

```sql

SELECT Name

FROM Employee

WHERE DeptID <> 1;

```

Employee Table:

| ID  | NAME   | DEPT_ID |
| --- | ------ | ------- |
| 1   | JOHN   | NULL    |
| 2   | GEORGE | 2       |
| 3   | SMITH  | 1       |
| 4   | RAY    | NULL    |

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

- There are 3 Employees (John, George and Ray) not in Dept 1. But Query returns only one result: George.
- Since we are just looking for employees not in Dept 1, query does not compare DeptID with NULL. So Employees without a department are not returned.

Correct Query is as follows:

```sql

SELECT Name

FROM Employee

WHERE DeptID IS NULL

OR DeptID <> 1;

```

</blockquote>

 </details>

51. Predict the output of the following query?

![Medium](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg>)

Consider following tables:

Employee:

| ID  | EMP_NAME |
| --- | -------- |
| 1   | JANE     |
| 2   | GEORGE   |
| 3   | JOHN     |

Department:

| ID  | DEPT_NAME  | EMP_NAME |
| --- | ---------- | -------- |
| 1   | MARKETING  | 1        |
| 2   | FINANCE    | 2        |
| 3   | TECHNOLOGY | NULL     |

  ```sql
  
SELECT \*

FROM Employee

WHERE id NOT IN (SELECT Emp_id

FROM Department)
  
  ```

<details>

<summary><b> Show Answer </summary></b>

<blockquote>

The above query will return no records. The reason for this is presence of null value in Emp_id column of Department table.

When we do SELECT Emp_id FROM Department, we get null value also. Now in main query we compare NOT IN with null value, then it does not return any result.

```sql

The correct query is:

SELECT \*

FROM Employee

WHERE id NOT IN (SELECT Emp_id

FROM Department WHERE Emp_id IS NOT NULL)

```

</blockquote>

</details>

---

52. Why do SQL queries need escape characters?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Show Answer </summary></b>

<blockquote>

- There are specific special characters and words reserved for specific purposes in SQL. For example, the reserved letter &.
- We must employ escape characters to send the message to the database telling it to interpret the special characters as non-special or non-reserved when we want to use them in the context of our data.

</blockquote>

</details>

---

53. Create a query to locate every employee from a employee list, whose name contains the term "Rich." For example: Rich, RICH, Rich.

![Medium](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg>)

<details>

<summary><b>Show Answer </b></summary>

<blockquote>

- We can use UPPER function for comparing the both sides with uppercase.

```sql

SELECT \*

FROM Employees

WHERE UPPER(emp_name) like '%RICH%'

```

</blockquote>

</details>

---

54. Create a SQL query To locate employees that has duplicate email ID.

![Medium](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg>)

Employee table:

| ID  | NAME    | EMAIL           |
| --- | ------- | --------------- |
| 10  | FREK    | MISHI@GMAIL.COM |
| 20  | RICHARD | ADAMS@GMAIL.COM |
| 30  | RAM     | MISHI@GMAIL.COM |

<details>

<summary><b> Show Answer</b></summary>

<blockquote>

We can use Group by clause on the column in which we want to find duplicate values.

```sql

Query would be as follows:

SELECT name, `COUNT`(email)

FROM Employee

GROUP BY email

HAVING ( COUNT(email) > 1 )

```

</blockquote>

 </details>
  
  ---
  

55. Write a SQL question to seek out records in Table A that aren't in Table B while not mistreatment NOT IN operator.
    Consider 2 tables

![Medium](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg>)

| TABLE A |
| ------- |
| 10      |
| 20      |
| 30      |

| TABLE B |
| ------- |
| 15      |
| 30      |
| 45      |

<details>

<summary><b>Show Answer </b></summary>

<blockquote>

- We can use `MINUS` operator during this case for Oracle and apart from SQL Server.

```sql

Query can be as follows:

SELECT _ FROM Table_A
MINUS
SELECT _ FROM Table_B

```

</blockquote>

</details>

---

56. What could be used instead of `distinct` in SQL?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

`GROUP BY` is meant for combination perform use; `DISTINCT` simply removes duplicates (based on all column values matching on a per row basis) from visibility. If TABLE2 permits duplicate values associated to TABLE1 records, you've got to use either choice.

</blockquote>

</details>

---
  
57. What is the Output for the following command?
  
  ```sql
INSERT INTO class VALUES(2, 'Rashid');

COMMIT;

UPDATE class SET name = 'Albert' WHERE id = '2';

SAVEPOINT A;

INSERT INTO class VALUES(3, 'Charlie');

SAVEPOINT B;

INSERT INTO class VALUES(4, 'Brandon');

SAVEPOINT C;

SELECT \* FROM class;
```

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

| id  | Name    |
| --- | ------- |
| 2   | Albert  |
| 3   | Charlie |
| 4   | Brandon |

</blockquote>

<details>

<summary><b>Explanation</b></summary>

- The Above commands is inserting values into a table class.
- `COMMIT` command is used to make sure that the data is stored permanently.
- Then the Name is being modified using `UPDATE` Command.
- `SAVEPOINT` is used to save that data at the certain point of time.
- The `SELECT` command is used to view the data in the table.

</details>

</details>

---

58. Spot the error in the given SQL query:

```sql
    Insert into Table Example( col1 [datatype],col2 [datatype],col3[datatype])
    values(val1,val2,val3);
    commit;
    rollback;
```

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

`ROLLBACK` command is not applicable if `COMMIT` is used before the usage of `ROLLBACK` Command.

</blockquote>

<details>

<summary><b>Explanation</b></summary>

<blockquote>

`COMMIT` command is used to store a data in the table permanently, therefore once the `COMMMIT` command is being executed there is no way for `ROLLBACK`.

</blockquote>

</details>

</details>

---

59. Which TCL Command is to be used for the below received output?

```SQL
CREATE TABLE Players(
ID INT,
First_Name VARCHAR(255),
Last_Name VARCHAR(255),
Date_Of_Birth date,
Place_Of_Birth VARCHAR(255),
Country VARCHAR(255),
PRIMARY KEY (ID)
);

insert into Players values(1, 'Jonathan', 'Swift', DATE('1981-04-22'), 'CapeTown', 'SouthAfrica');<br>
insert into Players values(2, 'Kumara', 'Sangakkara', DATE('1977-10-27'), 'Matale', 'Srilanka'); <br>
________;
insert into Players values(1, 'Mahendra Singh', 'Dhoni', DATE('1981-07-07'), 'Ranchi', 'India');<br>
```

O/P:

| ID  | First_Name     | Last_Name | Date_Of_Birth | Place_Of_Birth | Country |
| --- | -------------- | --------- | ------------- | -------------- | ------- |
| 1   | Mahendra Singh | Dhoni     | 1981-07-07    | Ranchi         | India   |

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

`ROLLBACK` is the missing Command

</blockquote>

<details>

<summary><b>Explanation</b></summary>

<blockquote>

- Based on the output, we can see that the insertion of the first 2 columns has been removed, Only the insertion below the missing command hence the missing command is `ROLLBACK`.

</blockquote>

</details>

</details>

---





  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  

