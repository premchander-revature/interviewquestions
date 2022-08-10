

1.Write a Query to create a table for the Students along with three columns of ID,NAME and DEPARTMENT.

<details>
<summary> Show Answer </summary>

```sql
CREATE TABLE Students (ID int,NAME varchar(30), DEPARTMENT varchar(30));
```

Explantion: The CREATE Command is used for creating a table  along with their variables(Column_Name) and Data Types(INT,VARCHAR(20)). 

</details>

<!--|Alter Query|-->

2.Write a Query to rename the table name from Employees to Employees_List.


|Table: Employees|

|First_Name | Last_Name 	| Birth_Date    | 	 Gender | 	 Joining_Date   |
|-----------|---------------|---------------|-----------|-------------------|
| Ajay		| Kumar	 	    | Mar-15-1970 	|       M  	| 	   Apr-05-2017  |
| David	 	| Richard 	    | Feb-17-1985 	|       M 	| 	   Mar-05-2017  |
| Junaid 	| M 	 	    | Sep-28-1987 	|       M 	| 	   Mar-09-2016  |
| Janvi	 	| Gowda 	 	| Oct-22-1993 	|       F 	| 	   Apr-09-2015  |
| Shobika	| Kumar	 	    | Aug-22-1996 	|       F 	| 	   Apr-15-2014  |



<details>
<summary> Show Answer </summary>

```sql
ALTER TABLE Employees RENAME TO Employees_List;
```
Explantion: Alter table is used for renaming the given table from one table name to another table name.


</details>


<!--|Alter Query|-->
3.Write a Query to alter the column name from Birth_Date to Date_of_Birth

|Table: Employees|

|First_Name | Last_Name 	| Birth_Date    | 	 Gender | 	 Joining_Date   |
|-----------|---------------|---------------|-----------|-------------------|
| Ajay		| Kumar	 	    | Mar-15-1970 	|       M  	| 	   Apr-05-2017  |
| David	 	| Richard 	    | Feb-17-1985 	|       M 	| 	   Mar-05-2017  |
| Junaid 	| M 	 	    | Sep-28-1987 	|       M 	| 	   Mar-09-2016  |
| Janvi	 	| Gowda 	 	| Oct-22-1993 	|       F 	| 	   Apr-09-2015  |
| Shobika	| Kumar	 	    | Aug-22-1996 	|       F 	| 	   Apr-15-2014  |

<details>
<summary> Show Answer </summary>

```sql
ALTER TABLE Employees_List RENAME COLUMN Birth_Date to Date_of_Birth;
```

Explantion: Alter table is used for renaming the given table from one column_name to another column_name.

</details>


4.Write a Query to adds a new column Location to the Employees_List table.

|Table: Employees|

|First_Name | Last_Name 	| Birth_Date    | 	 Gender | 	 Joining_Date   |
|-----------|---------------|---------------|-----------|-------------------|
| Ajay		| Kumar	 	    | Mar-15-1970 	|       M  	| 	   Apr-05-2017  |
| David	 	| Richard 	    | Feb-17-1985 	|       M 	| 	   Mar-05-2017  |
| Junaid 	| M 	 	    | Sep-28-1987 	|       M 	| 	   Mar-09-2016  |
| Janvi	 	| Gowda 	 	| Oct-22-1993 	|       F 	| 	   Apr-09-2015  |
| Shobika	| Kumar	 	    | Aug-22-1996 	|       F 	| 	   Apr-15-2014  |


<details>
<summary> Show Answer </summary>

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

Explantion: Alter table is used for Addition of a new column_name in  the given table .

</details>


5.Write a Query to drops a column Joining_Date to the Employees table.

|Table: Employees|

|First_Name | Last_Name 	| Birth_Date    | 	 Gender | 	 Joining_Date   |
|-----------|---------------|---------------|-----------|-------------------|
| Ajay		| Kumar	 	    | Mar-15-1970 	|       M  	| 	   Apr-05-2017  |
| David	 	| Richard 	    | Feb-17-1985 	|       M 	| 	   Mar-05-2017  |
| Junaid 	| M 	 	    | Sep-28-1987 	|       M 	| 	   Mar-09-2016  |
| Janvi	 	| Gowda 	 	| Oct-22-1993 	|       F 	| 	   Apr-09-2015  |
| Shobika	| Kumar	 	    | Aug-22-1996 	|       F 	| 	   Apr-15-2014  |

<details>
<summary> Show Answer </summary>

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


Explanation: Alter Table is used for Addition of a new column_name in  the given table and droping(Deleting) the coulumn_name from the given table.

</details>

6.Write a statement to adds a primary key on the First_Name column in the given table.

|Table: Employees|

|First_Name | Last_Name 	| Birth_Date    | 	 Gender | 	 Joining_Date   |
|-----------|---------------|---------------|-----------|-------------------|
| Ajay		| Kumar	 	    | Mar-15-1970 	|       M  	| 	   Apr-05-2017  |
| David	 	| Richard 	    | Feb-17-1985 	|       M 	| 	   Mar-05-2017  |
| Junaid 	| M 	 	    | Sep-28-1987 	|       M 	| 	   Mar-09-2016  |
| Janvi	 	| Gowda 	 	| Oct-22-1993 	|       F 	| 	   Apr-09-2015  |
| Shobika	| Kumar	 	    | Aug-22-1996 	|       F 	| 	   Apr-15-2014  |

<details>
<summary> Show Answer </summary>

```sql
ALTER TABLE Employees ADD PRIMARY KEY (First_Name);
```

Explanation: Primary Key uniquely identifes each record in a table and a table can have only one primary key.
</details>

7.Write a Query to Create a table Groceries_List along with 4 columns having Grocery_Id, Grocery_Name, Quantity , Price and add a primary key in Grocery_Id.

<details>
<summary> Show Answer </summary>

```sql
CREATE TABLE Groceries_List (Grocery_Id int ADD PRIMARY KEY, Grocery_Name VARCHAR(30), Quantity INT, Price TEXT);
```
Explanation: Creating a table name Groceries_List and adding a primary key in (Grocery_Id int ADD PRIMARY KEY) because only one primary key is allowed in a given table.
</details>


8.Write a Syntax for the CREATE TABLE AS statement in SQL.

<details>

<summary> Show Answer </summary>

```sql
CREATE TABLE [ IF NOT EXISTS ] new_table [ AS ] 
  SELECT expressions
  FROM existing_tables
  [WHERE conditions];
```


</details>


9.What is Primary key?

<details>
<summary> Show Answer </summary>

Explanations:

- Primary key is a field or the combination of fields that uniquely identify the each record in the table.
- If the column contains primary key, it cannot be null or empty.
- It cannot have more than one primary key.
- It stores uniques values into column. For Example, the Employee ID can be treated as the primary key for a Employees in Company.

</details>


10.Assemble a table to hold data on weather monitoring cities having latitude_north,longitude_west and temprature with NO duplicate ID fields are allowed.

<details>
<summary> Show Answer </summary>

```sql
CREATE TABLE WEATHER_MONITOR (ID INT PRIMARY KEY, CITY VARCHAR(30), STATE VARCHAR(30), TEMP REAL, LATITUDE_N REAL, LONGITUDE_W REAL);
```

Explanation: 

Create a table along with a table name "WEATHER_MONITOR" contains fields such as ID with the datatype INTEGER, CITY with the datatype VARCHAR, STATE with the datatype VARCHAR, TEMPERATURE, LATITUDE_N, LONGITUDE_W with the datatype REAL.Duplicates are not allowed as ID is declared as Primary Key.


</details>




11.How to delete the column Latitude_N and Longitude_W from the table WEATHER_MONITOR

<details>
<summary> Show Answer </summary>

``` sql

ALTER TABLE WEATHER_MONITOR DROP COLUMN LATITUDE_N;
ALTER TABLE WEATHER_MONITOR DROP COLUMN LONGITUDE_W;
```

Explanation:

    Deletion of column using DROP Command, it deletes the column along with the data.
    DROP command removes a whole database or just a table.

</details>

12.Write a short note on relational model.

<details>
<summary> Show Answer </summary>

- The relational model uses a collection of tables to represent both data and the relationships
among those data. 
- The relational model is an example of a record based model.

</details>

13. Find out the following error given in the table:


create table Student(Stu_Id int, Stu_Name varchar(20), Age int, Grade Varchar(5), City varchar(20), parent_mobileno int);

          
<details>
<summary> Show Answer </summary>

create table Student(Stu_Id int, Stu_Name varchar(20), Age int, Grade Varchar(5), City varchar(20), parent_mobileno text);

    |  Stu_Id |    Stu_Name      | Age | Grade |     City      | parent_mobileno |
    |---------|------------------|-----|-------|---------------|-----------------|
    |    1    |     Arthi        |  15 |   B   |     Andhra    |   9876573453    |
    |    2    |     Ganga        |  18 |   D   |    Bangalore          7865432190    |                                
          |    3    |   Madhumitha     |  17 |   A   |     Delhi     |   9092456778    |                          
          |    4    |    RIYA SREE     |  10 |   C   |     Kerala    |   8906758763    |                                
	      |    5    |  PRIYA GANESH    |  20 |   B   |     Chennai   |	 7689543213    |

Explanation: In this command the column_name and data type of parent_mobileno will be in the data type (int) it will not be accepted but it takes the data type (text)for the parent_mobileno .

</details>

14.How many tables may be included with a Join?
- a. One 
- b. Two
- c. Three
- d. All of the above.

<details>
<summary> Show Answer </summary>

Correct Answer: D
Explanation: The maximum number of tables that can be referenced in a single join is 61. 

</details>

15.A view can be deleted with the _________ command.
- a. DELETE VIEW
- b. TRUNCATE VIEW 
- c. REMOVE VIEW
- d. DROP VIEW  

<details>
<summary> Show Answer </summary>

Correct Answer: D
- Explanation: DROP VIEW removes one or more views from the current database.

</details>

16.Which command is used to delete columns from a table?
- a. MODIFY TABLE TableName DROP ColumnName
- b. ALTER TABLE TableName DROP COLUMN ColumnName
- c. ALTER TABLE TableName DROP ColumnName
- d. MODIFY TABLE TableName DROP COLUMN ColumnName
<details>

<summary> Show Answer </summary>

Correct Answer: B

- Explanation: 

* The ALTER TABLE command adds, deletes, or modifies columns in a table.
* The ALTER TABLE command also adds and deletes various constraints in a table.

</details>

17.Which Command can be used to add columns to a table?
- a. MODIFY TABLE TableName ADD ColumnName
- b. ALTER TABLE TableName ADD COLUMN ColumnName
- c. ALTER TABLE TableName ADD ColumnName
- d. MODIFY TABLE TableName ADD COLUMN ColumnName

<details>

<summary> Show Answer </summary>
Correct Answer: C

Explanation: 
    The ALTER TABLE statement is used to add, delete, or modify columns in an existing table. The ALTER TABLE statement is also used to add and drop various constraints on an existing table. 

</details>

18.Which command is used to remove all data from a table?
- a. DELETE
- b. TRUNCATE
- c. REMOVE
- d. Both A and C

<details>
<summary> Show Answer </summary>

Correct Answer: b

Explanation: 
Delete and Remove:
The DELETE command is used to delete specified rows(one or more).
Truncate:
The TRUNCATE command is used to delete all the data from a table.

</details>

19.Write a query to create a new table with the same data and structure as an existing table.

<details>

<summary> Show Answer </summary>

Syntax:

CREATE TABLE New_Table_Name SELECT * FROM Existing_Table_Name;  

Example: The following query creates Student_Marks table from the existing Student table:

CREATE TABLE Student_Marks SELECT * FROM Student;

Explanation: Here we use two tables (Student_Marks and  Student) so first  we take Student_Marks table from the existing Student table already.

</details>

20.Write a Query to add another column in the existing table:

<details>
<summary> Show Answer </summary>

Syntax:

ALTER TABLE Table_Name ADD Column_Name Datatype ( Length_of_Column) ;  


Example:

The following query adds the Stu_Address column to the existing Student table:

ALTER TABLE Student ADD Stu_Address varchar (25) ;  

OUTPUT:
|  Student_ID  |  	Stu_Name    |	Stu_Subject_ID  |	Stu_Marks  |	Stu_Age  |   Stu_Address  |
|     101	   |    Bharathi    |      Bsc102       |	   75	   |      21	 |      NULL      |
|     102	   |    Sandhiya    |	   BE104	    |      89      |	  20	 |      NULL      |
|     103	   |     Pooja	    |      Bsc102	    |      43	   |      20	 |      NULL      |
|     104	   |     Vinoth	    |      Bsc102	    |      56      |	  21	 |      NULL      |
|     107	   |    Shreemathi  |	   BCA103       |	   98      |	  22	 |      NULL      |

Explanation: 
    If you want to add another column or field to the existing table, you must use the ALTER statement in SQL.	
    </details>


21.In spite of allowing the removal of every row from a database, this operation flushes a table more quickly because rollback information is not stored.

A. Create  command
B. Truncate command
C. Drop table command
D. Alter table command
<details>
<summary> Show Answer </summary>

Correct Answer : B

Explanation: 
     An existing table's whole contents can be deleted using the SQL TRUNCATE TABLE command. You can also use the DROP TABLE command to completely remove a table from the database, but doing so would need you to recreate the table in order to continue storing data.

</details>


22.The command used to delete a specific column in a relation is__________.
A. ALTER , DROP 
B. TRUNCATE COLUMN
C. UPDATE TABLE
D. DELETE COLUMN

<details>
<summary> Show Answer </summary>

Correct Ans : A
Explanation: 
The command used to remove a specific column from a relation is ALTER, DROP.

</details>

23.How to set Primary key using Alter command?

<details>
<summary> Show Answer </summary>

Correct Answer:

Syntax: 

ALTER TABLE EmployeeDetail ADD PRIMARY KEY (P_EmployeeID)

Explanation: 
You cannot define a primary key for a table that already has one since a table can only have one primary key. Using a DROP clause in an ALTER TABLE statement, remove the current primary key from the table and replace it with the new main key.

</details>
   