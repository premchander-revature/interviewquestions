# DDL commands



1.What is Data Definition Language ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- The structure of database objects in a database can be created and modified using a computer language called a data definition language. 
- Views, schemas, tables, indexes, and other database objects are among them. 
- In a database table, it describes the fields and records.

</blockquote>

</details>

--------

2.List out the types of DDL commands which is used in sql.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

`CREATE` - The database or any of its objects, such as tables, indexes, functions, views, store procedures, and triggers, are created using the `CREATE` command. <br>
`DROP` -  Objects can be removed from the database using the `DROP` command. <br>
`ALTER` - The database structure can be changed using the `ALTER` command. <br>
`TRUNCATE` - `TRUNCATE` is used to delete every record from a table, together with any spaces set aside for the records.<br>
`COMMENT` - To add comments to a data dictionary, use the command `COMMENT`. <br>
`RENAME` - `RENAME` is used to rename an existing database object. <br>

</blockquote>

</details>

-------

3.Write a SQL query to create a table for the students that contains three columns as ID,NAME and DEPARTMENT.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
CREATE TABLE Students (ID INT,NAME VARCHAR(30), DEPARTMENT VARCHAR(30));
```

</blockquote>

<details>
<summary><b>Explanation</b></summary>

<blockquote>

The `CREATE` Command is used for creating a table along with their variables(Column_Name) and Data Types(INT,VARCHAR(20)). 

</blockquote>

</details>
</details>

------

4.How can we copy the existing table and use it for the development purposes without changing the real table ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
CREATE TABLE table_name AS (SELECT select_query);
```

</blockquote>

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

5.How could we copy the table structure excluding the data from the existing table ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
CREATE TABLE table_name AS (SELECT * FROM old_table WHERE 1=0);
```

</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- We can use the `CTAS` for copy the table's structure along with the `WHERE` clause in the `SELECT` query to ensure there are no rows to be return.

</blockquote>

</details>
</details>

------

6.How can we copy the table structure with some columns from the existing table?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
CREATE TABLE table_name1 AS (SELECT table_no, first_name, last_name FROM table_name);
```

</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- We can use the `CTAS` to copy the table's structure along with the `WHERE` clause in the `SELECT` query to ensure to select particular columns.

</blockquote>

</details>
</details>

-------

7.How to create an event and write a sample query for the annual function in the office?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
CREATE EVENT event_name 
ON SCHEDULE AT CURRENT_TIMESTAMP + INTERVAL 1 HOUR 
DO 
UPDATE myschema.mytable SET mycol = mycol +1 ;
```
</blockquote>

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

8.Assemble a table to hold data on weather monitoring cities having latitude_north,longitude_west and temprature with NO duplicate ID fields are allowed.

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>

```sql
CREATE TABLE WEATHER_MONITOR (ID INT PRIMARY KEY, CITY VARCHAR(30), STATE VARCHAR(30), TEMP REAL, LATITUDE_N REAL, LONGITUDE_W REAL);
```

</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

Create a table along with a table name "WEATHER_MONITOR" contains fields such as ID with the datatype `INTEGER`, CITY with the datatype `VARCHAR`, STATE with the datatype `VARCHAR`, TEMPERATURE, LATITUDE_N, LONGITUDE_W with the datatype `REAL`.

</blockquote>

</details>
</details>

-------

9.How to create a new database and view the database which is already added in it?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>

```sql
CREATE DATABASE database_name;
```

```sql
SHOW DATABASES;
```

</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- Creation of database is easy in sql by using `CREATE` `DATABASE` command followed by the databse name.
- When you create a database you can see the list of all databases which is created by you in the system. <br>
E.g List of Databases

| Databases      |
|----------------|
| Weather Report |
| Finance        |
            
            
</blockquote>

</details>
</details>

-----

10.How to check the database if already created in the system? Write a Sample query.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>

```sql
CREATE DATABASE IF NOT EXISTS database_name;
```
</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- The above syntax is used to create a database which is not already exist in the system adding `IF`
`NOT` `EXISTS`

</blockquote>

</details>
</details>

-------

11.Which of the following defines a `VIEW`?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a. Shorter form of a table. <br>
b. It is the logical representation of the subsets from one or more tables. <br>
c. It has only one row and one column <br>
d. None of the above <br>

<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>
b.It is the logical representation of the subsets from one or more tables.
</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- A `VIEW` is a virtual table and it contains rows and columns just like a real table.

</blockquote>

</details>
</details>

-------

12.What does database objects contain ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.Sequence <br>
b.Table <br>
c.Synonym <br>
d.All of the above <br>

<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>
d.All of the above
</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- Sequence, Table and Synonym are the database objects which are physically stored in database schema.

</blockquote>

</details>
</details>

-------

13.Which of the following database objects gives an alternative name to an object?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.Synonym <br>
b.Sequence <br>
c.View <br>
d.Index <br>

<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>
a.Synonym
</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- A permanent alias for the database object is known as a synonym.
- Any database user has access to a public synonym.
- The user who created a private synonym is the only one who may access it.

</blockquote>

</details>
</details>

-------

14. Which of the following database object is used to improve the performance of queries?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.Table <br>
b.Synonym <br>
c.View <br>
d.Index <br>

<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>
c.Index
</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- The database search engine can speed up data retrieval by using indexes, which are specialised lookup tables. 
- An index can be thought of as a pointer to information in a table.
- The index in the back of a book is nearly identical to an index in a database.
</blockquote>

</details>
</details>

-------

15.What is the range of number of letters in a table name?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.1-30 characters <br>
b.1-20 characters <br>
c.1-10 characters <br>
d.1-40 characters <br>

<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>
a.1-30 characters
</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- A table name can have only upto 30 characters limit.
</blockquote>

</details>
</details>

-------

16.Which of the following special characters cannot be used in table name ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.# <br>
b.@ <br>
c.$ <br>
d._ <br>

<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>
b. @
</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- #,$, _ are the only special characters can be used in table name.
</blockquote>

</details>
</details>

-------

17.While creating a table which of the following option can be use with the `DEFAULT` option ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.Strings<br>
b.SQL functions<br>
c.Expressions<br>
d.All of the above<br>

<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>
d. All of the above
</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- A default value specifies the column by using the keyword `DEFAULT`.
</blockquote>

</details>
</details>

------

18.What command is used to view a table's structure?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.`UPDATE`<br>
b.`SHOW`<br>
c.`SPOOL`<br>
d.`DESCRIBE`<br>

<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>

d. `DESCRIBE`

</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- To see the structure of the table by using the command `DESCRIBE`.

</blockquote>

</details>
</details>

------

19.Which of the following statement refers to both table and index?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.A table and an index cannot be the same name in a schema.<br>
b.A table and an index can have the same name in a schema.<br>
c.Neither A nor B<br>
d.None of the above<br>


<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>

b. A table and an index can have the same name in a schema

</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- In Sql, both table and index can have the same name also the index and contraints share the same namespace.

</blockquote>

</details>
</details>

------

20.In which of the following query used to create a table with no rows?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

```sql
a. CREATE TABLE stu AS SELECT 0 from students;
```
```sql
b. CREATE TABLE stu AS SELECT * from students where 1=1;
```
```sql
c. CREATE TABLE stu AS SELECT * from students where 1=0;
```
```sql
d. CREATE TABLE stu AS SELECT 0 from students;
```

<details>
<summary> <b> Show Answer </b> </summary>

<blockquote>

```sql
CREATE TABLE stu AS SELECT * from students where 1=0;
```
</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- By using `CTAS` can be use to copy the structure of the existing table without copying any data.

</blockquote>

</details>
</details>

------

21.Write a query to rename the table name from Employees to Employees_List.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

|Table: Employees|

|First_Name | Last_Name 	| Birth_Date    | 	 Gender | 	 Joining_Date   |
|-----------|---------------|---------------|-----------|-------------------|
| Ajay		| Kumar	 	    | Mar-15-1970 	|       M  	| 	   Apr-05-2017  |
| David	 	| Richard 	    | Feb-17-1985 	|       M 	| 	   Mar-05-2017  |
| Junaid 	| M 	 	    | Sep-28-1987 	|       M 	| 	   Mar-09-2016  |
| Janvi	 	| Gowda 	 	| Oct-22-1993 	|       F 	| 	   Apr-09-2015  |
| Shobika	| Kumar	 	    | Aug-22-1996 	|       F 	| 	   Apr-15-2014  |


<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
ALTER TABLE Employees RENAME TO Employees_List;
```
</blockquote>

<details>
<summary> <b> Explanation </b> </summary>

<blockquote>

- To rename the table name using `RENAME` along with the `ALTER` command.

</blockquote>

</details>
</details>

------

22.Write a query to alter the column name from Birth_Date to Date_of_Birth

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

|Table: Employees|

|First_Name | Last_Name 	| Birth_Date    | 	 Gender | 	 Joining_Date   |
|-----------|---------------|---------------|-----------|-------------------|
| Ajay		| Kumar	 	    | Mar-15-1970 	|       M  	| 	   Apr-05-2017  |
| David	 	| Richard 	    | Feb-17-1985 	|       M 	| 	   Mar-05-2017  |
| Junaid 	| M 	 	    | Sep-28-1987 	|       M 	| 	   Mar-09-2016  |
| Janvi	 	| Gowda 	 	| Oct-22-1993 	|       F 	| 	   Apr-09-2015  |
| Shobika	| Kumar	 	    | Aug-22-1996 	|       F 	| 	   Apr-15-2014  |

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
ALTER TABLE Employees_List RENAME COLUMN Birth_Date to Date_of_Birth;
```
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- `ALTER TABLE` command is used for renaming the given table from one column_name to another column_name.

</blockquote>

</details>
</details>

------

23.Write a query to adds a new column Location to the Employees_List table.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

|Table: Employees|

|First_Name | Last_Name 	| Birth_Date    | 	 Gender | 	 Joining_Date   |
|-----------|---------------|---------------|-----------|-------------------|
| Ajay		| Kumar	 	    | Mar-15-1970 	|       M  	| 	   Apr-05-2017  |
| David	 	| Richard 	    | Feb-17-1985 	|       M 	| 	   Mar-05-2017  |
| Junaid 	| M 	 	    | Sep-28-1987 	|       M 	| 	   Mar-09-2016  |
| Janvi	 	| Gowda 	 	| Oct-22-1993 	|       F 	| 	   Apr-09-2015  |
| Shobika	| Kumar	 	    | Aug-22-1996 	|       F 	| 	   Apr-15-2014  |


<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
ALTER TABLE Employees ADD (Location varchar(30));
```


|First_Name | Last_Name 	| Birth_Date    | 	 Gender | 	 Joining_Date   |Location|
|-----------|---------------|---------------|-----------|-------------------|--------|
| Ajay		| Kumar	 	    | Mar-15-1970 	|       M  	| 	   Apr-05-2017  |Null    |
| David	 	| Richard 	    | Feb-17-1985 	|       M 	| 	   Mar-05-2017  |Null    |
| Junaid 	| M 	 	    | Sep-28-1987 	|       M 	| 	   Mar-09-2016  |Null    |
| Janvi	 	| Gowda 	 	| Oct-22-1993 	|       F 	| 	   Apr-09-2015  |Null    |
| Shobika	| Kumar	 	    | Aug-22-1996 	|       F 	| 	   Apr-15-2014  |Null    |

</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- By using `ALTER TABLE` command is used for Addition of a new column_name in  the given table followed by the table name.

</blockquote>

</details>
</details>

------


24.Write a query to delete a column Joining_Date in the Employees table.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

|Table: Employees|

|First_Name | Last_Name 	| Birth_Date    | 	 Gender | 	 Joining_Date   |
|-----------|---------------|---------------|-----------|-------------------|
| Ajay		| Kumar	 	    | Mar-15-1970 	|       M  	| 	   Apr-05-2017  |
| David	 	| Richard 	    | Feb-17-1985 	|       M 	| 	   Mar-05-2017  |
| Junaid 	| M 	 	    | Sep-28-1987 	|       M 	| 	   Mar-09-2016  |
| Janvi	 	| Gowda 	 	| Oct-22-1993 	|       F 	| 	   Apr-09-2015  |
| Shobika	| Kumar	 	    | Aug-22-1996 	|       F 	| 	   Apr-15-2014  |

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
ALTER TABLE Employees_List DROP column Joining_Date;
```

|First_Name | Last_Name 	| Birth_Date    | 	 Gender | 	
|-----------|---------------|---------------|-----------|
| Ajay		| Kumar	 	    | Mar-15-1970 	|       M  	| 	 
| David	 	| Richard 	    | Feb-17-1985 	|       M 	| 	 
| Junaid 	| M 	 	    | Sep-28-1987 	|       M 	| 	 
| Janvi	 	| Gowda 	 	| Oct-22-1993 	|       F 	| 	  
| Shobika	| Kumar	 	    | Aug-22-1996 	|       F 	| 	  

</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- To delete a particular column in the table using `DROP` followed `ALTER TABLE` command in sql.

</blockquote>

</details>
</details>

------

25.Write a statement to adds a primary key on the First_Name column in the given table.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

|Table: Employees|

|First_Name | Last_Name 	| Birth_Date    | 	 Gender | 	 Joining_Date   |
|-----------|---------------|---------------|-----------|-------------------|
| Ajay		| Kumar	 	    | Mar-15-1970 	|       M  	| 	   Apr-05-2017  |
| David	 	| Richard 	    | Feb-17-1985 	|       M 	| 	   Mar-05-2017  |
| Junaid 	| M 	 	    | Sep-28-1987 	|       M 	| 	   Mar-09-2016  |
| Janvi	 	| Gowda 	 	| Oct-22-1993 	|       F 	| 	   Apr-09-2015  |
| Shobika	| Kumar	 	    | Aug-22-1996 	|       F 	| 	   Apr-15-2014  |

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
ALTER TABLE Employees ADD PRIMARY KEY (First_Name);
```
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>
- Primary Key uniquely identifes each record in a table and a table can have only one primary key.
</blockquote>

</details>
</details>

------

26.In Which of the following below querie used to add a column in a table which is already created?


![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

```sql
a. ALTER TABLE table_name add column (place varchar2(20));
```
```sql
b. ALTER TABLE table_name add place varchar2(20);
```
```sql
c. ALTER TABLE table_name add column (place);
```
```sql
d. ALTER TABLE table_name add (place varchar2(20));
```

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
d. ALTER TABLE table_name add (place varchar2(20));
```
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- `ALTER TABLE` command used to add a new column to a table. New column should define by a column name and datatype. 

</blockquote>

</details>
</details>

------

27.What command is used to modify the datatype which is already existed in a column?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/medium%20(2).svg)

```sql
a. ALTER TABLE table_name MODIFY place varchar2(10);
```
```sql
b. ALTER TABLE table_name MODIFY (place varchar2(10));
```
```sql
c. ALTER TABLE table_name MODIFY column (place varchar2(10));
```
```sql
d. ALTER TABLE table_name MODIFY (place varchar2(10));
```

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
d. ALTER TABLE table_name MODIFY (place varchar2(10));
```
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- `ALTER TABLE` & `MODIFY` command used to modify the column in a table by changing the datatype.
</blockquote>

</details>
</details>

------

28.Which is the vaild query to delete the column from the table ?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/medium%20(2).svg)

```sql
a. ALTER TABLE table_name DROP (place varchar2(20) );
```
```sql
b. ALTER TABLE table table_name DROP COLUMN (place);
```
```sql
c. ALTER TABLE table table_name DROP COLUMN (place) varchar2(20));
```
```sql
d. ALTER TABLE table_name MODIFY (place varchar2(20));
```

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
b. ALTER TABLE table table_name DROP COLUMN (place);
```
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- `ALTER TABLE` & `DROP` command used to delete the column from the table.
</blockquote>

</details>
</details>

------

29.Let us consider the following schema below

STUDENTS(sub_code, dep_name, location_id, city);

Which code snippet will modify the STUDENTS table and add an address column with the data type `VARCHAR2(100)`?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/medium%20(2).svg)

```sql
a. ALTER TABLE students ADD COLUMN(address varchar2(100));
```
```sql
b. ALTER TABLE students ADD (address varchar2(100));
```
```sql
c. MODIFY TABLE students ADD COLUMN (address varchar2(100));
```
d. None of the above.

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
b. ALTER TABLE students ADD (address varchar2(100));
```
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- `ALTER TABLE` & `ADD` command used to add the column address in the students table.

</blockquote>

</details>
</details>

------

30.In which of the following code snippet will delete a view named marks_maths?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/medium%20(2).svg)

```sql
a. delete view marks_maths;
```
```sql
b. delete marks_maths;
```
```sql
c. drop view marks_maths;
```
```sql
d. drop marks_maths;
```

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
c. drop view marks_maths;
```
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- `DROP` command used to remove the column marks_maths in the  table.

</blockquote>

</details>
</details>

------

31.What is temp tables ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Temporary tables are introduced by SQL server. It can create at runtime and do all operations that the normal table can do. 
- Temporary tables are present inside the tempdb database.

</blockquote>

</details>

------

32.What happens if the table is dropped ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- The structure of the table, relatioship, constraints and access privileges are all together will get dropped when using `DROP` command in the table.

</blockquote>

</details>

------

33.What are the  functional differences do `DROP` and `TRUNCATE` have?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- The DROP command is used to delete all of the data in a table or database, including any indexes and data. In contrast, the TRUNCATE command is used to remove all of the table's rows.

</blockquote>
</details>

------

34.What is Primary key?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary>  <b>Explanation</b> </summary>

<blockquote>

- Primary key is a field or the combination of fields that uniquely identify the each record in the table.
- If the column contains primary key, it cannot be null or empty.
- It cannot have more than one primary key.
- It stores uniques values into column. For Example, the Employee ID can be treated as the primary key for a Employees in Company.

</blockquote>

</details>

------

35.Why we need a index if the primary key is present already in the table?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary>  <b>Explanation</b> </summary>

<blockquote>

- The Database Engine enforces the data's uniqueness when we define a primary key in a table by generating a unique index for those columns.
- This is helps to improves the data retrieval when a primary key is used in queries.
- So we need to create an index even if a primary key is already present.

</blockquote>

</details>

------

36.Find the debug in the following query below?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

```sql
CREATE TABLE emp AS SELECT * FROM employees HAVING 1=0; 
```

<details>
<summary>  <b>Show Answer</b> </summary>

<blockquote>

```sql
CREATE TABLE emp AS SELECT * FROM employees WHERE 1=0; 
```
</blockquote>
<details>
<summary>  <b>Explanation</b> </summary>

<blockquote>

- `WHERE` clause can be used to select the rows while copying the data from one table instead of `HAVING` clause.

</blockquote>
</details>
</details>

------

37.Find the debug in the following query below?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

```sql
ALTER TABLE table_name add (city int(20));
```

<details>
<summary>  <b>Show Answer</b> </summary>

<blockquote>

```sql
ALTER TABLE table_name add (city VARCHAR(20)); 
```
</blockquote>

<details>
<summary>  <b>Explanation</b> </summary>

<blockquote>

- "city" column cannot be a integer datatype we have to mention a `VARCHAR` datatype.

</blockquote>
</details>
</details>

------


38.Find the debug in the following query below?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

```sql
ALTER TABLE table_name drop city;
```

<details>
<summary>  <b>Show Answer</b> </summary>

<blockquote>

```sql
ALTER TABLE table_name DROP column city; 
```
</blockquote>

<details>
<summary>  <b>Explanation</b> </summary>

<blockquote>

- While deleting the column need to mention the `drop` command along with column and column_name.

</blockquote>
</details>
</details>

------

39.A `DROP TABLE` command can be a rollback ? Say True or False.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary>  <b>Show Answer</b> </summary>

<blockquote>
False
</blockquote>

<details>
<summary>  <b>Explanation</b> </summary>

<blockquote>

- A `DROP TABLE` command cannot be a rollback in sql.

</blockquote>
</details>
</details>

------

40.Why should we use a view in sql ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary>  <b>Explanation</b> </summary>

<blockquote>

- A view is used to restrict access to the data, making simple queries from complex and giving a different views of same data.

</blockquote>
</details>

------

41.How to quickly obtain records from a table and give an explanation.

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

42.What will happen if the statement's DEFAULT clause provision is deleted?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

Table will be created with no default value for CREATE_DATE column

</blockquote>
</details>

------

43.You are designing a table for the Bank department.In which datatype you need to store an interval of days, hours, minutes and seconds in a column.?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>

<blockquote>

INTERVAL YEAR TO MONTH

</blockquote>
</details>

------

44.What about making a table is true?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- It's not necessary to mention a table's size. Online table editing is possible. 
- To create the table's structure, each column needs attributes such data kinds and precision.

</blockquote>
</details>

------

45.What emerges if a transaction is in effect against a table on which a DDL is issued?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- The transaction is committed and terminated
- The current transaction will be committed and stopped if a DDL statement is used. The current transaction will make permanent all database modifications. The DDL statement refers to this as an implicit commit.

</blockquote>
</details>

------


46.What is schema and its reliablity?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- A schema in a SQL database is a list of logical data structures. The schema, which shares the same name as the database manager, is owned by a database user.
- It consists of a group of database items related to a database.

</blockquote>
</details>

------

47.By using quoted Identifiers ' ', you could create tables. In what manner will you reference the table?

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

48.What is accurate regarding a table obtained by a sub-query? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- When a table is made using a sub-query, a LONG column is not replicated.
- The LONG column is not copied when a table is created using the CTAS (CREATE TABLE AS SELECT) method.

</blockquote>
</details>

------

49.How you determine the referenced data when you delete the parent record.

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

50.How can we copy the existing table and use it for the development purposes without changing the real table ?

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

51.How to create an event and write a sample query for the annual function in the office ?

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

52.You need to add a constraint to the EMPLOYEES table which restricts the addition of those employees who have salaries less than 10000.

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

53.Write a query for the employee table having ID, first_name, last_name, salary, joining_date, department_id along with a Inline foreign key.?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql
CREATE TABLE employee ( employee_id NUMBER(20), first_name VARCHAR(150), last_name VARCHAR(150), salary NUMBER(10), hire_date DATE, department_id NUMBER(10) CONSTRAINT fk_emp_deptid REFERENCES department(dept_id) );
```
</blockquote>

<details>
<summary><b>Explanation</b></summary>

<blockquote>

- Creating the table along with the table name having columns id, first_name, last_name, salary, joining_date and placing foreign key in  department_id 

</blockquote>

</details>
</details>

------
