1.Write a query to fetch values in table Sample_a that are and not in Sample_b without using the NOT keyword.

  Given two tables created as follows:

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

select _ from Sample_a
except
select _ from Sample_b;

```

</blockquote>
</details>

---

2.Find the Error in the given SQL query:

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

<summary> Explanation </summary>
<blockquote>

    In the above query we use GROUP BY MARKS means, it clusters the rows with same Marks and we also use SELECT MARKS, COUNT(DISTINCT STUDENT_ID) which prints the Marks of each cluster and the count of rows of respective clusters. 

</blockquote>

</details>
</details>

---


3.Find the Error in the given query:

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

<summary> Explanation </summary>
<blockquote>

    The expression BillingYear in the WHERE clause is invalid. Even though it is defined as an alias in the SELECT phrase, which appears before the WHERE phrase, the logical processing order of the phrases of the statement is different from the written order.

</blockquote>
</details>
</details>

---

4.Which of the following query finds the names of the sailors who have reserved atleast one boat?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.SELECT DISTINCT s.name FROM sailors , reserves WHERE s.sid = r.sid;

b.SELECT s.sname FROM sailors s ,reservers r WHERE s.sid = r.sid;

c.SELECT DISTINCT s.name FROM sailors s, reserves r WHERE s.sid = r.sid;

d.None of these

<details>
<summary> Show Answer </summary>
<blockquote>

C.SELECT DISTINCT s.name FROM sailors s, reserves r WHERE s.sid = r.sid;

</blockquote>

</details>

---

5.After the completion of a transaction in SQL, it must be executed to save all the operations performed in the transaction. Here we are talking about which command?

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

<summary> Explanation </summary>
<blockquote>

 The COMMIT command must be executed to save all the operations performed in the transaction.

</blockquote>
</details>

---

6.Which of the following SQL statement is valid?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)


a.SELECT \_ FROM Employees WHERE Gender = 'F';

b.SELECT \_ FROM Employees;

c.SELECT Gender= 'M' FROM Employees;

d.SELECT Gender FROM Employees WHERE Last_Name = 'Gowda';

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

7.Write the sql query to get the employee details using last name ?

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

By using SELECT key in addition to WHERE clause to be used for Last_Name

</blockquote>

</details>
</details>

---

8.Decide which statement is true.

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

- Data definition language (DDL) refers to the set of SQL commands that can create and manipulate the structures of a database. DDL statements are used to create, change, and remove objects including indexes, triggers, tables, and views.

</blockquote>
</details>
</details>

---

9.Which statement is used to get all data from the student table whose name starts with p?

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
- The \_ symbol is used to match exactly one character. Therefore option C is the correct choice.
</blockquote>
</details>
</details>

---

10.Table Employee has 10 Records,it has a non - NULL SALARY column which is also UNIQUE.Predict the output. 

For the SQL statement

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

# DDL Commands Interview Questions


11.What functional differences do Drop and Truncate have?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- The DROP command is used to delete all of the data in a table or database, including any indexes and data. In contrast, the TRUNCATE command is used to remove all of the table's rows.

</blockquote>
</details>

------

12.How to quickly obtain records from a table and give an explanation.

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

14.You are designing a table for the Bank department.In which datatype you need to store an interval of days, hours, minutes and seconds in a column.?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

INTERVAL YEAR TO MONTH

</blockquote>
</details>

------

15.What about making a table is true?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- It's not necessary to mention a table's size. Online table editing is possible. 
- To create the table's structure, each column needs attributes such data kinds and precision.

</blockquote>
</details>

---

16.What emerges if a transaction is in effect against a table on which a DDL is issued?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- The transaction is committed and terminated
- The current transaction will be committed and stopped if a DDL statement is used. The current transaction will make permanent all database modifications. The DDL statement refers to this as an implicit commit.

</blockquote>
</details>

---


17.What is schema and its reliablity?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- A schema in a SQL database is a list of logical data structures. The schema, which shares the same name as the database manager, is owned by a database user.
- It consists of a group of database items related to a database.

</blockquote>
</details>

------

18.By using quoted Identifiers ' ', you could create tables. In what manner will you reference the table?

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

20.How you determine the referenced data when you delete the parent record.

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

21.How can we copy the existing table and use it for the development purposes without changing the real table ?

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

22.How to create an event and write a sample query for the annual function in the office ?

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

23.Assemble a table to hold data on weather monitoring cities having latitude_north,longitude_west and temprature with NO duplicate ID fields are allowed.

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

24.Query to look at table WEATHER_MONITOR in undefined order in sql.

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


25.You need to add a constraint to the EMPLOYEES table which restricts the addition of those employees who have salaries less than 10000.

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

27.Which Command is used to temporarily save a transaction so that you can rollback to that point whenever necessary?

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

30.How to reduce the Data redundancy in a database ?

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
  
 
  
  
  
  
  
  49. Write a query for this problem?

Given the Employee table, where each employee has a DeptId, To transfer personnel from DeptID 1 to DeptID 2 and from DeptID 2 to DeptID 1, use a single SQL query.

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

Table: Employee

| ID  | NAME   | DEPT_ID |
| --- | ------ | ------- |
| 1   | JOHN   | 1       |
| 2   | GEORGE | 2       |
| 3   | JANE   | 1       |
| 4   | SMITH  | 2       |

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

50. What is wrong with this request for the list of workers who don't work for Dept. 1?

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

## </details>

51. What will be the result of following query?

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

SELECT \*

FROM Employee

WHERE id NOT IN (SELECT Emp_id

FROM Department)

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

53. Create a query to locate every employee, regardless of case, whose name contains the term "Rich." As in Rich, RICH, Rich.

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

54. To locate employees that have multiple emails, create a query.

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

- We can use MINUS operator during this case for Oracle and apart from SQL Server.

```sql

Query can be as follows:

SELECT _ FROM Table_A
MINUS
SELECT _ FROM Table_B

```

</blockquote>

</details>

---

56. What will be used rather than distinct in SQL?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

GROUP BY is meant for combination perform use; DISTINCT simply removes duplicates (based on all column values matching on a per row basis) from visibility. If TABLE2 permits duplicate values associated to TABLE1 records, you've got to use either choice.

</blockquote>

</deatils>

```



```

  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  

