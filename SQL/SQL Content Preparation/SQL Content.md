SQL CONTENT BASED QUESTIONS:

DEFINITION BASED QUESTIONS:

1.What is database?

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

A database is an organized collection of data.

</blockquote>

</details>

---

2.What is DBMS?

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

DBMS stands for Database Management system. It is a software that controls the creation, maintenance and use of a database.

</blockquote>

</details>

---

3.Name two DBMS Software.

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Two DBMS Software are :

1. MySQL

2. Oracle

3. Microsoft SQL Server

4. Microsoft Access.

</blockquote>

</details>

---

4.What is the difference between Flat file and Relational ?

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

| Flat File                                                            | Relational                                                                      |
| -------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| Data is stored in a single table. Data is stored in multiple tables. | It is suitable for less amount of data. It is suitable for large amount of data |

</blockquote>

</details>

---

5.Write four advantages of database.

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Four advantages of database are

1. It reduces Data Redundancy

2. It allows sharing of data.

3. It help to maintain data integrity.

4. It provides Data Security.

</blockquote>

</details>

---

6.What do you mean by Data Redundancy?

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Duplication of data in a database is known as data redundancy.

</blockquote>

</details>

---

7.What do you mean by Data Integrity?

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Data integrity means that the data is accurate and consistent in the database.

</blockquote>

</details>

---

8.What is Data Consistency?

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Data Consistency means there should be multiple mismatching copies of the same data in a database.

</blockquote>

</details>

---

9.Write two features of database.

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Two features of database are :

1. A database can have one or many tables.

2. Every table in a database has a primary key field which ensures 00% unique values in the database.

</blockquote>

</details>

10. What do you mean by RDBMS.

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

RDBMS stands for Relational Database Management System. When data is to be stored, maintained, and retrieved from multiple tables then special database software are required known as RDBMS.

</blockquote>

</details>

---

11.What is Primary Key?

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

A field which is unique for each and every record in a table is called primary key.

</blockquote>

</details>

---

12.What do you mean by Composite Primary key?

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

When primary key constraint is applied on one or more columns then it is known as Composite Primary Key.

</blockquote>

</details>

---

13.What is Foreign Key?

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Ans:A Foreign Key is a field in one table that refers to the primary key of another table. It is used to link two tables.

</blockquote>

</details>

---

EXERCISE:STUDENT

14.Answer the following questions on the basis of following table:

Table : Student

| Stud_id | Stud_name | Class | Fees |
| ------- | --------- | ----- | ---- |
| 1       | Aman      | IX    | 3000 |
| 2       | Anil      | X     | 3200 |

Table Teacher

| T_id | T_name   | T_Sal | Stud_id |
| ---- | -------- | ----- | ------- |
| 3210 | Mr.Kumar | 60000 | 1       |
| 3211 | Mr.Sethi | 70000 | 2       |

1.Identify the primary key in Student and Teacher table.
2.Identify the foreign key in Teacher table.

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

1. Primary Key in Student table : Stud_id
   Primary key in Teacher table is : T_id

2. Foreign key in Teacher table is : Stud_id

</blockquote>

</details>

---

15. Multiple tables can be created in a database. (T / F)

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

True

</blockquote>

</details>

---

16. \_\_\_\_\_ are the basic building blocks of a database

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Tables

</blockquote>

</details>

---

17. What is the default data type of a field while creating table in design view?

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Varchar

</blockquote>

</details>

---

18. Write four appropriate field names and their data types to store record of book.

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Four appropriate field names and their data types to store record of book are :

a. Author_name ————- Char / Varchar

b. Price ———————– Float / Decimal / Double

c. Class ———————– Char / Varchar

d. Subject ———————Char / Varchar

</blockquote>

</details>

---

19. Write four appropriate field names and their data types to store record of student.

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Four appropriate field names and their data types to store record of students are :

1. Name —————> Char / Varchar

2. Admno —————> Integer

3. Fees ————–> Float/Double

4. DOB —————> Date

</blockquote>

</details>

---

20.Write four data types which are used to store numerical value.

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Four data types which are used to store numerical value are
Smallint
Bigint
Integer
Float

</blockquote>

</details>

---

21. In RDBMS table is also known as \_\_\_\_

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Relation

</blockquote>

</details>

---

22. Data in a (RDBMS) is organized in the form of \_\_\_\_\_.

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Tables

</blockquote>

</details>

---

23. Write four data types available in Alphanumeric Data types

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Four data types available in Alphanumeric Data types :

- LongVarchar
- Char
- Varchar
- Varchar_Ignorecase

</blockquote>

</details>

---

24.Write the data type suitable for the following fields.

a. DateofBirth

b. Name

c. Rollno

d. Class

e. Email

f. City

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

a. DateofBirth – Date

b. Name – Char or Varchar

c. Rollno – TinyInt / Smallint / Integer

d. Class – Char / Varchar

e. Email – Char or Varchar

f. City – Char or Varchar

</blockquote>

</details>

---

25. Define the following terms :

i)   Table

ii)  Fields

iii) Records

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Table : A table is a set of data elements that is organized in vertical columns and horizontal rows.

Fields : A field is a set of data values of a particular simple type, one for each row of the table.

Records : A row also called a Record or Tuple represents a single, data item in a table.

</blockquote>

</details>

---

26.What do you mean by query in Open Office Base?

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

A query is a request to collect specific information from a table or combination of tables.

 </blockquote>

 </details>

---

27.In how many ways you can create query in Open Office Base?

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

We can create query in Open Office Base by three ways which are :

- Create query in Design view
- Create query using Wizard
- Create query in SQL view

</blockquote>

</details>

---

28.Name the Query language which is used in Base?

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SQL

 </blockquote>

 </details>

---

29.Which command is used to retrieve data from the table?

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select command is used to retrieve data from the table.

</blockquote>

</details>

---

30.Name two categories of SQL Commands

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Two categories of SQL Commands are :

- DDL
- DML

</blockquote>

</details>

---

31.Differentiate between DDL and DML Commands.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

| DDL                                    | DML                                      |
| -------------------------------------- | ---------------------------------------- |
| It stands for Data Definition Language | It stands for Data Manipulation Language |
| Example : Create, Alter, Drop          | Example : Insert, Update, Delete         |

</blockquote>

</details>

---

32.Identify the DML Commands from the following :

1.Create
2.Alter
3.Insert
4.Delete

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Insert and Delete are the DML Commands

</blockquote>

</details>

---

33. ________ is the most commonly used Data Manipulation Language(DML) command.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select

</blockquote>

</details>

---

34. Name two clauses which can be used with Select Command.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Two clauses which can be used with Select Command are :

- Where Clause
- Order By Clause

</blockquote>

</details>

---

35. Write the Select command to display all the records of table “book”.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from book;

</blockquote>

</details>

---

36. Write the shortcut to execute query in “Create query in SQL view” of Base.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

F5

 </blockquote>

 </details>

---

37. What is the purpose of Where clause in Select Command?

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Where Clause is used to retrieve specific record from the table.

</blockquote>

</details>

---

38. What is the purpose of Order by clause in Select Command?

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Order by clause is used to arrange the records in ascending or descending order.

</blockquote>

 </details>

---

Exercise:

39. Write the queries for the following table : Emp

<blockquote>
 
| Emp_id | Ename  | Salary |
|--------|--------|--------|
| 1      | Suman  | 20000  |
| 2      | Sanjay | 32000  |
| 3      | Ravi   | 30000  |

</blockquote>

</details>

a. Display the salary of all the employees after incrementing by Rs 1000.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select Salary +1000 from Emp;

</blockquote>

</details>

b. Display the Employee id and salary of all the employees after decreasing by Rs 500.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select Emp_id, Salary – 500 from Emp;

</blockquote>

</details>

c.Display the Name and salary of all the employees after incrementing it as thrice the amount of present salary.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select Ename, Salary \* 3 from Emp;

</blockquote>

</details>

d.Display the Employee id, Name and salary of all the employees after decrementing it as half the amount of present salary.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select Emp_id, Ename, Salary/2 from Emp;

</blockquote>

</details>

e.Display the Employee id and Name of all the employees.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select Emp_id, Ename from Emp;

</blockquote>

</details>

---

Exercise: "STUDENT"

40.Write the queries for the following table : Student

| Admno | Name   | Class | House  |
| ----- | ------ | ----- | ------ |
| 1001  | Sonam  | 9     | Blue   |
| 1002  | Ravi   | 10    | Yellow |
| 1003  | Poonam | 10    | Green  |

a.Display the entire tabl

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Student

</blockquote>

</details>

b.Display the list of students whose house color is blue.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Student where House = “Blue”

</blockquote>

</details>

c.Display the admission number of students whose house color is green.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select Admno from Student where House = “Yellow”

</blockquote>

</details>

d.To view records in ascending order of Admission Number.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Student order by Admno Asc;

</blockquote>

</details>

e.Display the records of Class 10 Students.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from students where Class = 10;

</blockquote>

</details>

f.Display the class of ‘Ravi’

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select Class from Student where Name = ‘Ravi’

</blockquote>

</details>

g. Insert the given record : 1004, “Aman”, 11, “Blue”

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Insert into Student values( 1004, “Aman”, 11, “Blue”)

</blockquote>

</details>

---

41.Which command is used for the following task in database?

- To insert a new record

- To modify the existing data.

- To delete a record

- To display record

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

- Insert
- Update
- Delete
- Select

</blockquote>

</details>

---

Exercise:"ITEM"

42. Write the queries for the following table : Item

| Itemno | Iname    | Price | Qty |
| ------ | -------- | ----- | --- |
| 12     | Pen      | 10    | 17  |
| 13     | Eraser   | 5     | 15  |
| 14     | Notebook | 15    | 20  |

a. Write a query to insert a new record of following details
15, “Pencil”, 20, 10

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Insert into Item values(15, “Pencil”, 20, 10)

</blockquote>

</details>

b.Write a query to display detail of items whose quantity is more than 10.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Item where Qty > 10

</blockquote>

</details>

c.Write a query to change the quantity of Item number 13 to 25.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Update Item set Qty = 25 where Itemno = 13

</blockquote>

</details>

d.Display the total amount of each item. The amount must be calculated as the price multiplied by quantity for each item

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select Price \* Qty from Item.

</blockquote>

</details>

e.Display the name of item whose price is 10.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select Iname from Item where price = 10

</blockquote>

</details>

f.Display all the records in ascending order of price.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Item order by Price asc.

</blockquote>

</details>

g.Identify the Primary key from table Item.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Itemno

</blockquote>

</details>

h.Write the suitable data type of field “Iname”.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Char or Varchar

</blockquote>

</details>

i.Write a query to increase the price of all items by Rs2.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Update Item set Price = Price + 2;

</blockquote>

</details>

j.Write a query to decrease the price of all items by Rs2 whose price is less than 20.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Update Item set Price = Price – 2 where Price < 20;

</blockquote>

</details>

---

43. By default, data is arranged in \_\_\_\_ order using ORDER BY clause.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Ascending Order

</blockquote>

</details>

---

44. Which clause is used for the following:
    a. To display specific record.
    b. To display records in a particular order.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

a. Where Clause
b. Order by Clause

</blockquote>

</details>

---

45. In the given query which of the keyword has to be inserted?

INSERT INTO employee **\_** (1002,Joey,2000);

a) Table
b) Values
c) Relation
d) Field

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

b) Values

</blockquote>

<summary><b>Explanation</b></summary>

<blockquote>

Value keyword has to be used to insert the values into the table.

</blockquote>

</details>

---

46.Which of the following statements contains an error?

a) Select \* from emp where empid = 10003;
b) Select empid from emp where empid = 10006;
c) Select empid from emp;
d) Select empid where empid = 1009 and lastname = ‘GELLER’;

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

d) Select empid where empid = 1009 and lastname = ‘GELLER’;

</blockquote>

<blockquote>

Explanation: This query do not have from clause which specifies the relation from which the values has to be selected.

</blockquote>

</details>

---

47.

| Employee_id | Name  | Salary |
| ----------- | ----- | ------ |
| 1001        | Annie | 6000   |
| 1009        | Ross  | 4500   |
| 1018        | Zeith | 7000   |

This is Employee table.
Which of the following employee_id will be displayed for the given query?

SELECT \* FROM employee WHERE employee_id>1009;
a) 1009, 1001, 1018
b) 1009, 1018
c) 1001
d) 1018

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

d) 1018

</blockquote>

<blockquote>

Greater than symbol does not include the given value unlike >=.

</blockquote>

</details>

---

48.This Query can be replaced by which one of the following?

```sql

 SELECT name, course_id
 FROM instructor, teaches
 WHERE instructor_ID= teaches_ID;

```

a) Select name,course_id from teaches,instructor where instructor_id=course_id;
b) Select name, course_id from instructor natural join teaches;
c) Select name, course_id from instructor;
d) Select course_id from instructor join teaches;

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

b) Select name, course_id from instructor natural join teaches;

</blockquote>

<blockquote>

Join clause joins two tables by matching the common column.

</blockquote>

</details>

---

49.The **\_\_\_\_** clause is used to list the attributes desired in the result of a query.

a) Where
b) Select
c) From
d) Distinct

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

b) Select

</blockquote>

<blockquote>

Explanation:

</blockquote>

</details>

---

50.The query given below will not give an error. Which one of the following has to be replaced to get the desired output?

```sql

   SELECT ID, name, dept name, salary * 1.1
   WHERE instructor;

```

a) Salary\*1.1
b) ID
c) Where
d) Instructor

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

c) Where

</blockquote>

<blockquote>

Where selects the rows on a particular condition. From gives the relation which involves the operation. Since Instructor is a relation it has to have from clause.

 </blockquote>

 </details>

---

51. The **\_\_** clause allows us to select only those rows in the result relation of the \_\_\_\_ clause that satisfy a specified predicate.

a) Where, from

b) From, select

c) Select, from

d) From, where

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

a) Where, from

</blockquote>

<blockquote>

Where selects the rows on a particular condition. From gives the relation which involves the operation.

</blockquote>

## </details>

52.Here which of the following displays the unique values of the column?

```sql

  SELECT ________ dept_name
   FROM instructor;

```

a) All

b) From

c) Distinct

d) Name

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

c) Distinct

</blockquote>

<blockquote>

Distinct keyword selects only the entries that are unique.

</blockquote>

</details>

---

53.

| Name   |
| ------ |
| Annie  |
| Bob    |
| Callie |
| Derek  |

Which of these query will display the the table given above ?
a) Select employee from name
b) Select name
c) Select name from employee
d) Select employee

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

c) Select name from employee

</blockquote>

<blockquote>

The field to be displayed is included in select and the table is included in the from clause.

</blockquote>

</details>

---

54. **\_** operator is used for appending two strings.
    a) &
    b) %
    c) ||
    d) \_

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

c) ||

</blockquote>

<blockquote>

|| is the concatenation operator.

 </blockquote>

 </details>

---

55.In SQL the spaces at the end of the string are removed by **\_\_\_** function.

a) Upper
b) String
c) Trim
d) Lower

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

c) Trim

</blockquote>

<blockquote>

The syntax of trim is Trim(s); where s-string.

</blockquote>

</details>

---

56. ```sql

    ```

SELECT instructor.\*
FROM instructor, teaches
WHERE instructor.ID= teaches.ID;

````

This query does which of the following operation?

a) All attributes of instructor and teaches are selected
b) All attributes of instructor are selected on the given condition
c) All attributes of teaches are selected on given condition
d) Only the some attributes from instructed and teaches are selected

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

b) All attributes of instructor are selected on the given condition

</blockquote>

<blockquote>

The asterisk symbol “ * ” can be usedin the select clause to denote “all attributes.”

</blockquote>

</details>

57. ``` sql

SELECT name
FROM instructor
WHERE salary <= 100000 AND salary >= 90000;

````

This query can be replaced by which of the following ?
a)

```sql

SELECT name
FROM instructor
WHERE salary BETWEEN 90000 AND 100000;
```

b)

```sql

SELECT name
FROM employee
WHERE salary <= 90000 AND salary>=100000;
```

c)

```sql

SELECT name
FROM employee
WHERE salary BETWEEN 90000 AND 100000;
```

d)

```sql

SELECT name
FROM instructor
WHERE salary BETWEEN 100000 AND 90000;
```

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

a)

```sql

SELECT name
FROM instructor
WHERE salary BETWEEN 90000 AND 100000;

```

<blockquote>

SQL includes a between comparison operator to simplify where clauses that specify that a value be less than or equal to some value and greater than or equal to some other value.

</blockquote>

</details>

---

58. ```sql

    ```

SELECT \*
FROM instructor
ORDER BY salary \_**_, name _**;

````

To display the salary from greater to smaller and name in ascending order which of the following options should be used?
a) Ascending, Descending
b) Asc, Desc
c) Desc, Asc
d) Descending, Ascending

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

c) Desc, Asc

</blockquote>

<blockquote>

Explanation:....

</blockquote>

---

59.``` sql

SELECT name
FROM instructor
WHERE dept name = ’Physics’
ORDER BY name;

````

By default, the order by clause lists items in **\_\_** order.
a) Descending
b) Any
c) Same
d) Ascending

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

d) Ascending

</blockquote>

<blockquote>

Specification of descending order is essential but it not for ascending.

</blockquote>

</details>

---

60. ’\_ \_ _ ’ matches any string of **\_\_** three characters. ’_ \_ \_ %’ matches any string of at **\_\_** three characters.

a) Atleast, Exactly
b) Exactly, Atleast
c) Atleast, All
d) All, Exactly

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

b) Exactly, Atleast

</blockquote>

<blockquote>

Explanation:

</blockquote>

</details>

---

61.``` sql
SELECT emp_name
FROM department
WHERE dept_name LIKE ’ **\_** Computer Science’;

````

Which one of the following has to be added into the blank to select the dept_name which has Computer Science as its ending string?
a) %
b) _
c) ||
d) $

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

a) %

</blockquote>

<blockquote>

The % character matches any substring.

</blockquote>

</details>

---

62.``` sql
SELECT * FROM employee WHERE dept_name="Comp Sci";
In the SQL given above there is an error . Identify the error.
````

a) Dept_name

b) Employee

c) “Comp Sci”

d) From

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

c) “Comp Sci”

</blockquote>

<blockquote>

For any string operations single quoted(‘) must be used to enclose.

 </blockquote>

 </details>

---

63. ```sql
    SELECT name ____ instructor name, course id
    FROM instructor, teaches
    WHERE instructor.ID= teaches.ID;
    ```

Which keyword must be used here to rename the field name?

a) From

b) Rename

c) As

d) Join

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

c) As

</blockquote>

<summary><b>Explanation</b></summary>

<blockquote>

As keyword is used to rename.

</blockquote>

</details>






























