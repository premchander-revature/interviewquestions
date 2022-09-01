<b>OVERALL JOINS QUESTIONS</b>

<b>DEFINITION BASED QUESTIONS:</b>

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

---

10. What do you mean by RDBMS.

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

RDBMS stands for Relational Database Management System. When data is to be stored, maintained, and retrieved from multiple tables then special database software are required known as `RDBMS`.

</blockquote>

</details>

---

11.What is Primary Key?

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

A field which is unique for each and every record in a table is called `primary key`.

</blockquote>

</details>

---

12.What do you mean by Composite Primary key?

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

When primary key constraint is applied on one or more columns then it is known as `Composite Primary Key`.

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

16. _______ are the basic building blocks of a database

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
   
- Smallint
- Bigint
- Integer
- Float

</blockquote>

</details>

---

21. In RDBMS,table is also known as __________

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

Relation

</blockquote>

</details>

---

22. Data in a (RDBMS) is organized in the form of __________

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

1. Table

1. Fields

1. Records

<details>

<summary><b> Show Answer </b></summary>

<blockquote>

- Table : A table is a set of data elements that is organized in vertical columns and horizontal rows.

- Fields : A field is a set of data values of a particular simple type, one for each row of the table.

- Records : A row also called a Record or Tuple represents a single, data item in a table.

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

33. _____ is the most commonly used Data Manipulation Language(DML) command.

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

36. Write the shortcut to execute query in `Create query in SQL view` of Base.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

F5

 </blockquote>

 </details>

---

37. What is the purpose of `Where` clause in Select Command?

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

`Where` Clause is used to retrieve specific record from the table.

</blockquote>

</details>

---

38. What is the purpose of `Order by` clause in Select Command?

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

`Order by` clause is used to arrange the records in ascending or descending order.

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

a.Display the entire table

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

j.Write a query to decrease the price of all items by Rs 2 whose price is less than 20.

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Update Item set Price = Price – 2 where Price < 20;

</blockquote>

</details>

---

43. By default, data is arranged in _______ order using `ORDER BY` clause.

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

49.The _______ clause is used to list the attributes desired in the result of a query.

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
   
<summary><b>Explanation</b></summary> 

<blockquote>

Where selects the rows on a particular condition. From gives the relation which involves the operation. Since Instructor is a relation it has to have from clause.

 </blockquote>

 </details>
   
 </details>

---

51. The ________ clause allows us to select only those rows in the result relation of the ______ clause that satisfy a specified predicate.

a) Where, from

b) From, select

c) Select, from

d) From, where

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

a) Where, from

</blockquote>
   
<summary><b>Explanation</b></summary>

<blockquote>

Where selects the rows on a particular condition. From gives the relation which involves the operation.

</blockquote>

</details>

---

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
   
<summary><b>Explanation</b></summary>

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
   
<summary><b>Explanation</b></summary>

<blockquote>

The field to be displayed is included in select and the table is included in the from clause.

</blockquote>

</details>

---

54. ______ operator is used for appending two strings.
   
    a) &
    b) %
    c) ||
    d) \_

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

c) ||

</blockquote>
   
<summary><b>Explanation</b></summary>

<blockquote>

|| is the concatenation operator.

 </blockquote>

 </details>

---

55.In SQL the spaces at the end of the string are removed by ________ function.

a) Upper
b) String
c) Trim
d) Lower

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

c) Trim

</blockquote>
   
<summary><b>Explanation</b></summary>

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
   
<summary><b>Explanation</b></summary>

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
   
<summary><b>Explanation</b></summary>

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
   
<summary><b>Explanation</b></summary>

<blockquote>

Explanation:

</blockquote>
   
</details>

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
   
<summary><b>Explanation</b></summary>

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
   
<summary><b>Explanation</b></summary>

<blockquote>

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

---

64.You can drop OUTER keyword and just say LEFT JOIN or RIGHT JOIN or FULL JOIN.

A) True

B) False

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

A) True

</blockquote>

<details>

<summary><b>Explanation</b></summary>

<blockquote>

</blockquote>

</details>

</details>

---

65.Use left or right outer join with _______ when you are looking for something in one table that doesn’t exist in another table.

A) null condition
B) inclusions
C) exclusions
D) none of above

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

C)exclusions

</blockquote>

<details>

<summary><b>Explanation</b></summary>

<blockquote>

Explanation:

</blockquote>

</details>

</details>

---

66.Understanding the primary and foreign key relationship is not important to join on the correct columns.

A) True
B) False

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

B) False

</blockquote>

<blockquote>

Explanation:

</blockquote>

</details>

---

67.A_____ is a query that retrieves rows from more than one table or view:
a) Start
b) End
c) Join
d) All of the mentioned

Answer: c
Explanation: An SQL join clause combines records from two or more tables in a database. It creates a set that can be saved as a table or used as it is. A JOIN is a means for combining fields from two tables by using values common to each.

---

68.LEFT JOIN and LEFT OUTER JOIN are equivalent.

A) True
B) False

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

A) True

 </blockquote>

 <blockquote>

Explanation:

</blockquote>

</details>

---

69.Self-JOIN can be attained by ........ based on requirement but table must join with itself.

A) INNER-JOIN
B) OUTER-JOIN
C) CROSS-JOIN
D) All of above
E) Both A & B

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

D) All of above

 </blockquote>

 <blockquote>

Explanation:

</blockquote>

</details>

---

70.Select the correct query/queries for cross join:

A)Select \* FROM Table1 T1 CROSS JOIN Table1 T2;

B)Select \* FROM Table1 T1 ALL CROSS JOIN Table1 T2;

C)Select \* FROM Table1 T1,Table1 T2;

D)Select \* FROM Table1 T1 CROSS Table1 T2;

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

A. Select \* FROM Table1 T1 CROSS JOIN Table1 T2;

</blockquote>

<blockquote>

Explanation:

</blockquote>

</details>

---

71.To avoid a Cartesian product, always include a valid join condition in a WHERE clause.

A) True
B) False

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

A)True

</blockquote>

<blockquote>

Explanation:

</blockquote>

</details>

---

72.EXERCISE PROBLEM:

SAMPLE TABLE- WORKER

| WORKER_ID | FIRST_NAME | LAST_NAME | SALARY | JOINING_DATE        | DEPARTMENT |
| --------- | ---------- | --------- | ------ | ------------------- | ---------- |
| 001       | Monika     | Arora     | 100000 | 2014-02-20 09:00:00 | HR         |
| 002       | Niharika   | Verma     | 80000  | 2014-06-11 09:00:00 | Admin      |
| 003       | Vishal     | Singhal   | 300000 | 2014-02-20 09:00:00 | HR         |
| 004       | Amitabh    | Singh     | 500000 | 2014-02-20 09:00:00 | Admin      |
| 005       | Vivek      | Bhati     | 500000 | 2014-06-11 09:00:00 | Admin      |
| 006       | Vipul      | Diwati    | 200000 | 2014-06-11 09:00:00 | Account    |
| 007       | Satish     | Kumar     | 75000  | 2014-01-20 09:00:00 | Account    |
| 008       | Geetika    | Chauhan   | 90000  | 2014-04-11 09:00:00 | Admin      |

SAMPLE TABLE- BONUS

| WORKER_REF_ID | BONUS_DATE          | BONUS_AMOUNT |
| ------------- | ------------------- | ------------ |
| 1             | 2016-02-20 00:00:00 | 5000         |
| 2             | 2016-06-11 00:00:00 | 3000         |
| 3             | 2016-02-20 00:00:00 | 4000         |
| 1             | 2016-02-20 00:00:00 | 4500         |
| 2             | 2016-06-11 00:00:00 | 3500         |

SAMPLE TABLE- TITLE

| WORKER_REF_ID | WORKET_TITLE | AFFECTED_FROM       |
| ------------- | ------------ | ------------------- |
| 1             | Manager      | 2016-02-20 00:00:00 |
| 2             | Executive    | 2016-06-11 00:00:00 |
| 8             | Executive    | 2016-06-11 00:00:00 |
| 5             | Manager      | 2016-06-11 00:00:00 |
| 4             | Asst.Manager | 2016-06-11 00:00:00 |
| 7             | Executive    | 2016-06-11 00:00:00 |
| 6             | Lead         | 2016-06-11 00:00:00 |
| 3             | Lead         | 2016-06-11 00:00:00 |

i)Write an SQL query to fetch “FIRST_NAME” from Worker table using the alias name as <WORKER_NAME>.

---

ii) Write an SQL query to fetch “FIRST_NAME” from Worker table in upper case.

---

iii)Write an SQL query to fetch unique values of DEPARTMENT from Worker table.

---

iv)Write an SQL query to print the first three characters of FIRST_NAME from Worker table.

---

v)Write an SQL query to find the position of the alphabet (‘a’) in the first name column ‘Amitabh’ from Worker table.

---

vi)Write an SQL query to print the FIRST_NAME from Worker table after removing white spaces from the right side.

---

vii)Write an SQL query to print the DEPARTMENT from Worker table after removing white spaces from the left side.

---

viii)Write an SQL query that fetches the unique values of DEPARTMENT from Worker table and prints its length.

---

ix)Write an SQL query to print the FIRST_NAME from Worker table after replacing ‘a’ with ‘A’.

---

x)Write an SQL query to print the FIRST_NAME and LAST_NAME from Worker table into a single column COMPLETE_NAME. A space char should separate them.

---

xi)Write an SQL query to print all Worker details from the Worker table order by FIRST_NAME Ascending.

---
xii)Write an SQL query to print all Worker details from the Worker table order by FIRST_NAME Ascending and DEPARTMENT Descending.

---

xiii)Write an SQL query to print details for Workers with the first name as “Vipul” and “Satish” from Worker table.

---

xiv)Write an SQL query to print details of workers excluding first names, “Vipul” and “Satish” from Worker table.

---

xv)Write an SQL query to print details of Workers with DEPARTMENT name as “Admin”.

---

xvi)Write an SQL query to print details of the Workers whose FIRST_NAME contains ‘a’.

---

xvii)Write an SQL query to print details of the Workers whose FIRST_NAME ends with ‘a’.

---

xviii)Write an SQL query to print details of the Workers whose FIRST_NAME ends with ‘h’ and contains six alphabets.

---

xix)Write an SQL query to print details of the Workers whose SALARY lies between 100000 and 500000.

---

xx)Write an SQL query to print details of the Workers who have joined in Feb’2014.

---

xxi)Write an SQL query to fetch the count of employees working in the department ‘Admin’.

---

xxii)Write an SQL query to fetch worker names with salaries >= 50000 and <= 100000.

---

xxiii)Write an SQL query to fetch the no. of workers for each department in the descending order.

---

xxiv)Write an SQL query to print details of the Workers who are also Managers.

---

xxv)Write an SQL query to fetch duplicate records having matching data in some fields of a table.

---

xxvi)Write an SQL query to show only odd rows from a table.

---

xxvii)Write an SQL query to show only even rows from a table.

---

xxviii)Write an SQL query to fetch intersecting records of two tables.

---

xxix)Write an SQL query to clone a new table from another table.

---

xxx)Write an SQL query to show records from one table that another table does not have.

---

xxxi)Write an SQL query to fetch the list of employees with the same salary.

---

xxxii)Write an SQL query to show the second highest salary from a table.

---

xxxiii)Write an SQL query to show one row twice in results from a table.

xxxiv)Write an SQL query to fetch intersecting records of two tables.

---

xxxv)Write an SQL query to fetch the first 50% records from a table.

xxxvi)Write an SQL query to show all departments along with the number of people in there.

xxxvii)Write an SQL query to show the last record from a table.

---

xxxviii)Write an SQL query to fetch the first row of a table.

xxxix)Write an SQL query to fetch three min salaries from a table.

---

ivL)Write an SQL query to fetch departments along with the total salaries paid for each of them.

---

Answers:

i)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select FIRST_NAME AS WORKER_NAME from Worker;

</blockquote>

</details>

---

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

ii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select upper(FIRST_NAME) from Worker;

</blockquote>

</details>

---

iii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select distinct DEPARTMENT from Worker;

</blockquote>

</details>

---

iv)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select substring(FIRST_NAME,1,3) from Worker;

</blockquote>

</details>

---

v)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select INSTR(FIRST_NAME, BINARY'a') from Worker where FIRST_NAME = 'Amitabh';

</blockquote>

</details>

---

vi)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select RTRIM(FIRST_NAME) from Worker;

</blockquote>

</details>

---

vii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select LTRIM(DEPARTMENT) from Worker;

</blockquote>

</details>

---

viii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select distinct length(DEPARTMENT) from Worker;

</blockquote>

</details>

---

ix)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select REPLACE(FIRST_NAME,'a','A') from Worker;

</blockquote>

</details>

---

x)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select CONCAT(FIRST_NAME, ' ', LAST_NAME) AS 'COMPLETE_NAME' from Worker;

</blockquote>

</details>

---

xi)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Worker order by FIRST_NAME asc;

</blockquote>

</details>

---

xii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Worker order by FIRST_NAME asc,DEPARTMENT desc;

</blockquote>

</details>

---

xiii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Worker where FIRST_NAME in ('Vipul','Satish');

</blockquote>

</details>

xiv)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Worker where FIRST_NAME not in ('Vipul','Satish');

</blockquote>

</details>

---

xv)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Worker where DEPARTMENT like 'Admin%';

</blockquote>

</details>

---

xvi)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Worker where FIRST_NAME like '%a%';

</blockquote>

</details>

---

xvii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Worker where FIRST_NAME like '%a';

</blockquote>

</details>

---

xviii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Worker where FIRST_NAME like '**\_**h';

</blockquote>

</details>

---

xix)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Worker where SALARY between 100000 and 500000;

</blockquote>

</details>

---

xx)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Worker where year(JOINING_DATE) = 2014 and month(JOINING_DATE) = 2;

</blockquote>

</details>

---

xxi)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT COUNT(\*) FROM worker WHERE DEPARTMENT = 'Admin';

</blockquote>

</details>

---

xxii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT CONCAT(FIRST_NAME, ' ', LAST_NAME) As Worker_Name, Salary
FROM worker
WHERE WORKER_ID IN
(SELECT WORKER_ID FROM worker
WHERE Salary BETWEEN 50000 AND 100000);

</blockquote>

</details>

---

xxiii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT DEPARTMENT, count(WORKER_ID) No_Of_Workers
FROM worker
GROUP BY DEPARTMENT
ORDER BY No_Of_Workers DESC;

</blockquote>

</details>

---

xxiv)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT DISTINCT W.FIRST_NAME, T.WORKER_TITLE
FROM Worker W
INNER JOIN Title T
ON W.WORKER_ID = T.WORKER_REF_ID
AND T.WORKER_TITLE in ('Manager');

</blockquote>

</details>

---

xxv)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT WORKER*TITLE, AFFECTED_FROM, COUNT(*)
FROM Title
GROUP BY WORKER*TITLE, AFFECTED_FROM
HAVING COUNT(*) > 1;

</blockquote>

</details>

---

xxvi)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT \* FROM Worker WHERE MOD (WORKER_ID, 2) <> 0;

xxvii)The required query is:

SELECT \* FROM Worker WHERE MOD (WORKER_ID, 2) = 0;

</blockquote>

</details>

---

xxviii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

(SELECT _ FROM Worker)
INTERSECT
(SELECT _ FROM WorkerClone);

</blockquote>

</details>

---

xxix)The general query to clone a table with data is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT \* INTO WorkerClone FROM Worker;

</blockquote>

</details>

The general way to clone a table without information is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT \* INTO WorkerClone FROM Worker WHERE 1 = 0;

</blockquote>

</details>

---

xxx)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT _ FROM Worker
MINUS
SELECT _ FROM Title;

</blockquote>

</details>

---

xxxi)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select distinct W.WORKER_ID, W.FIRST_NAME, W.Salary
from Worker W, Worker W1
where W.Salary = W1.Salary
and W.WORKER_ID != W1.WORKER_ID;

</blockquote>

</details>

---

xxxii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select max(Salary) from Worker
where Salary not in (Select max(Salary) from Worker);

</blockquote>

</details>

---

xxxiii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

select FIRST_NAME, DEPARTMENT from worker W where W.DEPARTMENT='HR'
union all
select FIRST_NAME, DEPARTMENT from Worker W1 where W1.DEPARTMENT='HR';

</blockquote>

</details>

---

xxxiv)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

(SELECT _ FROM Worker)
INTERSECT
(SELECT _ FROM WorkerClone);

</blockquote>

</details>

---

xxxv)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT \*
FROM WORKER
WHERE WORKER_ID <= (SELECT count(WORKER_ID)/2 from Worker);

</blockquote>

</details>

---

xxxvi)The following query returns the expected result:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT DEPARTMENT, COUNT(DEPARTMENT) as 'Number of Workers' FROM Worker GROUP BY DEPARTMENT;

</blockquote>

</details>

---

xxxvii)The following query will return the last record from the Worker table:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Worker where WORKER_ID = (SELECT max(WORKER_ID) from Worker);

</blockquote>

</details>

---

xxxviii)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Select \* from Worker where WORKER_ID = (SELECT min(WORKER_ID) from Worker);

</blockquote>

</details>

---

xxxix)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT distinct Salary from worker a WHERE 3 >= (SELECT count(distinct Salary) from worker b

</blockquote>

</details>

---

xL)The required query is:

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

SELECT DEPARTMENT, sum(Salary) from worker group by DEPARTMENT;

</blockquote>

</details>

---

73.Write SQL Query to get Student Name and number of Students in same grade.

Given Student Table

ID         | Name           | Grade

1          | George         | 1

2          | Smith          | 2

Answer: We can use WITH clause for this problem. We first get the number students in each grade by using GROUP BY on grade. Then we use Sub-Query returned by WITH clause in Main query.

Query will be as follows:

WITH grade_count AS (

  SELECT grade, COUNT(*) AS grade_count

  FROM   student

  GROUP BY grade)

SELECT s.name AS student_name,

       gc.grade_count AS grade_count

FROM   student s,

       grade_count gc

WHERE  e.grade = gc.grade;

---

74.Write SQL Query to get the list of grades with total score more than average score.

Consider Student and Grade tables

Student: ID, name, grade_ID, score

Grade: ID, grade_num

Answer: We can use WITH clause to get the total score in each grade. We can also use WITH clause to get the average score among all grades. Then we can use the two sub-queries to get the list of GRADES with Score total more than average score.

Query will be as follows:

WITH

  grade_score AS (

    SELECT grade_num, SUM(s.score) grade_total

    FROM   student s, grade g

    WHERE  s.grade_ID = g.ID

    GROUP BY grade_num),

  avg_score AS (

    SELECT SUM(grade_total)/COUNT(*) avg

    FROM   grade_score)

SELECT *

FROM   grade_score

WHERE  grade_total > (SELECT avg FROM avg_score) ORDER BY grade_num;

---

75.Write a SQL query to maximum Zipcode from a table without using MAX or MIN aggregate functions.

Consider Zipcode_list table with column Zipcode

ZIPCODE

7500

7525

7550

7600

7575

Answer: Point to be noted is that the Maximum zipcode is not smaller than any Zipcode in the list.

We can use self join to find the list of Zipcodes that are smaller than at least one other Zipcode. Once we get that list, we just use NOT IN to find the Zipcode from Zipcode_list that does not exist in this smaller list. That will be the maximum Zipcode with no Zipcode bigger than it.

Query will be as follows:

SELECT DISTINCT Zipcode

FROM Zipcode_list

WHERE Zipcode NOT IN (

SELECT Smaller_list.Zipcode

FROM Zipcode_list AS Larger_list

JOIN Zipcode_list AS Smaller_list

ON Smaller_list.Zipcode < Largerlist.Zipcode

)

---

76.Which SQL feature can be used to view data in a table sequentially?

In this question, we need to clarify with interviewer if it is about SEQUENCE based on some value in data or it is just a SEQUENCE of rows from data.

In first case, we can use ORDER BY clause in SQL to view data in a sequential order based on a value.

In second case, we can use a CURSOR to view the whole data set in a sequence.

---

77.These three tasks can be carried out using a SELECT statement:

- Choose rows from a table.
- Choose columns from a table.
- Bring together data that is stored in different tables by creating a link between them.

Which set of keywords describes these capabilities?

![Simple](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

A. difference, projection, join

B. selection, projection, join

C. Selection, intersection, join

D. Intersection, projection, join

<details><summary> <b>Show Answer</b> </summary>
<blockquote>
  
 B. selection, projection, join

</blockquote>
  
<details><summary> <b>Explanation</b> </summary>
<blockquote>
  
 selection, projection, join is the answer.
  
</blockquote></blockquote>
</details>

---

78.Test the following SQL statement: Which functions of a SELECT statement are carried out in the statement?
SELECT e.EMPLOYEE_ID,e.LAST_NAME,e.DEPARTMENT_ID, d.DEPARTMENT_NAME FROM EMP e, DEPARTMENT d WHERE e.DEPARTMENT_ID = d.DEPARTMENT_ID;

![Simple](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

A. Selection, projection, join

B. Difference, projection, join

C. Selection, intersection, join

D. Intersection, projection, join

<details><summary> <b>Show Answer</b> </summary>
  
> A. Selection, projection, join
  
<details><summary> <b>Explanation</b> </summary>
  
>In the statement, Selection, projection, join capabilities of a SELECT statement are performed
  
  </details>
</details>

---

79.What kind of join is the following SQL?
SELECT CUSTOMER_T. CUSTOMER_ID, ORDER_T. CUSTOMER_ID, NAME, ORDER_ID FROM CUSTOMER_T,ORDER_T

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

A. Equi-join
B. Natural join
C. Outer join
D. Cartesian join

<details><summary> <b>Show Answer</b> </summary>
  
> D. Cartesian join
  
<details><summary> <b>Explanation</b> </summary>
  
>Cartesian Join is simply the joining of one or more table which returns the product of all the rows in these tables.
  
  </details>
</details>

---

80.Which kind of join does the following SQL represent?

SELECT CUSTOMER_T. CUSTOMER_ID, ORDER_T. CUSTOMER_ID, NAME, ORDER_ID FROM CUSTOMER_T,ORDER_T WHERE CUSTOMER_T. CUSTOMER_ID = ORDER_T. CUSTOMER_ID

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

A. Equi-join
B. Natural join
C. Outer join
D. Cartesian join

<details><summary> <b>Show Answer</b> </summary>

A. Equi-join

<details><summary> <b>Explanation</b> </summary>
  
> Equi-join joins only same data entry field. For example, one table contains department id and another table should contain department id.
  
  </details>
</details>

---

81.Which of the subsequent statements is accurate?

![Simple](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

A. INNER JOIN only retrieves those rows from Cartesian Product that satisfy the JOIN condition
B. FULL OUTER JOIN is same as CROSS JOIN
C. SELF JOIN is a special type of OUTER JOIN
D. Both A and C

<details><summary> <b>Show Answer</b> </summary>

A. INNER JOIN only retrieves those rows from Cartesian Product that satisfy the JOIN condition

<details><summary> <b>Explanation</b> </summary>
  
> INNER JOIN only retrieves those rows from Cartesian Product that satisfy the JOIN condition is true.

  </details>
</details>

---

82.What is the FULL OUTER JOIN formed on two tables, Table1 and Table2, and which of the following statements about it is TRUE?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

A. Retrieves all the unmatched rows of Table1
B. Retrieves all the unmatched rows of Table2
C. Retrieves both matched and unmatched rows of Table1 and Table2
D. Retrieves only matched rows of table1 and Table2

<details><summary> <b>Show Answer</b></summary>

C. Retrieves both matched and unmatched rows of Table1 and Table2

<details><summary> <b>Explanation</b> </summary>
  
- The statement is TRUE about FULL OUTER JOIN created on two tables Table1 and Table2 is Retrieves both matched and unmatched rows of Table1 and Table2.

  </details>
</details>

---

83.Which view in the top-level FROM clause of the SELECT query contains more than one table:

![Complex](https://github.com/krishnagopika/githubpages/blob/main/hard.jpg)

A. Join view
B. Datable join view
C. Updatable join view
D. All of the mentioned

<details><summary> <b>Show Answer</b> </summary>

C. Updatable join view

<details><summary> <b>Explanation</b> </summary>
  
> Updatable join view that contains more than one table in the top-level FROM clause of the SELECT statement.

  </details>
</details>

---

84.A query that retrieves rows from many tables or views is known as a ______________

![Simple](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

A. Start
B. End
C. Join
D. All of the above

<details><summary> <b>Show Answer</b> </summary>

C. Join

<details><summary> <b>Explanation</b> </summary>
  
> A Join is a query that retrieves rows from more than one table or view.

  </details>
</details>

---

85.Only the relation previously mentioned preserves tuples using the left outer join

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

A. Right outer join operation
B. Right inner join operation
C. Left inner join operation
D. Left outer join operation

<details><summary> <b>Show Answer</b> </summary>

D. Left outer join operation

<details><summary> <b>Explanation</b> </summary>
  
>  Left outer join preserves tuples only in the relation named before Left outer join operation.

  </details>
</details>
   
---

86.Using the word inner is, how would you express a normal join?

![Simple](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

A. Mandatory
B. Optional
C. Independent
D. Free

<details><summary> <b>Show Answer</b> </summary>

B. Optional

<details><summary> <b>Explanation</b> </summary>
  
>  To specify a normal join, using the keyword inner is Optional.

  </details>
</details>

---

87.Which of the following claims is untrue?

![Simple](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

A. RIGHT OUTER JOIN is equivalent to LEFT OUTER JOIN if order of tables are reversed
B. FULL OUTER JOIN is same as CROSS JOIN
C. SELF JOIN is a special type of OUTER JOIN
D. Both B and C

<details><summary> <b>Show Answer</b> </summary>

D. Both B and C

<details><summary> <b>Explanation</b> </summary>
  
> Both B and C option are False statements.

  </details>
</details>

---

88.What join corresponds to the Cartesian product?

![Simple](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

A. INNER JOIN
B. OUTER JOIN
C. CROSS JOIN
D. NATURAL JOIN

<details><summary> <b>Show Answer</b> </summary>

C. CROSS JOIN

<details><summary> <b>Explanation</b> </summary>
  
>  CROSS JOIN is equivalent to Cartesian Product.

  </details>
</details>

---

89.Which of the following have to be true for INNER JOIN to function?

![Complex](https://github.com/krishnagopika/githubpages/blob/main/hard.jpg)

A. Columns used for joining must have same name
B. Columns used for joining can have same or different name
C. Columns used for joining must have different names
D. Columns used for joining must have different names

<details><summary> <b>Show Answer</b> </summary>

B. Columns used for joining can have same or different name

<details><summary> <b>Explanation</b> </summary>
  
> Columns used for joining can have same or different name is the following conditions has to be satisfied for INNER JOIN to work

  </details>
</details>

---

90.When the resultant table needs rows from A and B that match the condition and rows from A that do not satisfy the condition, which join between tables A and B should be used?

![Complex](https://github.com/krishnagopika/githubpages/blob/main/hard.jpg)

A. Outer Join
B. Cross Join
C. Inner Join
D. None of the above

<details><summary> <b>Show Answer</b> </summary>

A. Outer Join

<details><summary> <b>Explanation</b> </summary>
  
>Outer Join is to be used between two tables A and B when the resultant table needs rows from A and B that matches the condition and rows from A that does not match the condition.

  </details>
</details>

---

91.Ten tuples and five characteristics make up relation R1. Relation R2 has 7 characteristics and 0 tuples. How many tuples would the resulting set include if R1 and R2 were to achieve a CROSS JOIN?

![Complex](https://github.com/krishnagopika/githubpages/blob/main/hard.jpg)

A. 28
B. 10
C. 0
D. 35

<details><summary> <b>Show Answer</b> </summary>

C. 0

<details><summary> <b>Explanation</b> </summary>
  
>When a CROSS JOIN is achieved between R1 and R2, 0 tuples the resultant set will have.

  </details>
</details>

---

92.Which join refers to join records from the write table that have no matching key in the left table are include in the result set:

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

A. Left outer join
B. Right outer join
C. Full outer join
D. None of the above

<details><summary> <b>Show Answer</b> </summary>

B. Right outer join

<details><summary> <b>Explanation</b> </summary>
  
>Right outer join refers to join records from the write table that have no matching key in the left table are include in the result set.

  </details>
</details>

---

93.Which join types are there in a join condition:

![Simple](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

A. Cross join
B. Natural join
C. Join with USING clause
D. All of the mentioned

<details><summary> <b>Show Answer</b> </summary>

D. All of the mentioned

<details><summary> <b>Explanation</b> </summary>
  
>INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN, EQUIJOIN are the types of joins.

  </details>
</details>

---

94.How many join conditions are there?

![Simple](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

A. 2
B. 3
C. 4
D. 5

<details><summary> <b>Show Answer</b> </summary>

D. 5

<details><summary> <b>Explanation</b> </summary>
  
>INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN, EQUIJOIN.

  </details>
</details>

---

95.Which type of JOIN is used to returns all rows from right table and only matched rows from left table?

![Simple](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

A.INNER JOIN
B.RIGHT JOIN
C.FULL JOIN
D.LEFT JOIN

<details><summary> <b>Show Answer</b> </summary>

B.RIGHT JOIN

<details><summary> <b>Explanation</b> </summary>
  
>RIGHT JOIN is similar to LEFT JOIN. This join returns all the rows of the table on the right side of the join and matching rows for the table on the left side of the join.

  </details>
</details>

---

96.Which type of JOIN is used to returns all rows from left table and only matched rows from right table?

![Simple](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

A.INNER JOIN
B.RIGHT JOIN
C.FULL JOIN
D.LEFT JOIN

<details><summary> <b>Show Answer</b> </summary>

D.LEFT JOIN

<details><summary> <b>Explanation</b> </summary>
  
>The LEFT JOIN is a clause of the SELECT statement. The LEFT JOIN clause allows you to query data from multiple tables. The LEFT JOIN returns all rows from the left table and the matching rows from the right table.

  </details>
</details>

---

97.Which view in the top-level FROM clause of the SELECT query contains more than one table:
a) Join view
b) Datable join view
c) Updatable join view
d) All of the mentioned

Answer: c
Explanation: The DELETE statement is used to delete rows in a table. The UPDATE statement is used to update existing records in a table. The INSERT INTO statement is used to insert new records in a table.

---

98.What actions are permitted in a join view:
a) UPDATE
b) INSERT
c) DELETE
d) All of the mentioned

Answer: d
Explanation: The DELETE statement is used to delete rows in a table. The UPDATE statement is used to update existing records in a table. The INSERT INTO statement is used to insert new records in a table.

---

98.Which join means that the result set includes records from the write table for which there is no key match in the left table:
a) Left outer join
b) Right outer join
c) Full outer join
d) Half outer join

Answer: b
Explanation: A right outer join will return all the rows that an inner join returns plus one row for each of the other rows in the second table that did not have a match in the first table. It is the same as a left outer join with the tables specified in the opposite order.

---

99.Which is a join condition and includes an equality operator
a) Equijoins
b) Cartesian
c) Both Equijoins and Cartesian
d) None of the mentioned

Answer: a
Explanation: An equi-join is a specific type of comparator-based join, that uses only equality comparisons in the join-predicate.

---

100.Which item is returned when there is no join condition in the join query:
a) Equijoins
b) Cartesian
c) Both Equijoins and Cartesian
d) None of the mentioned

Answer: b
Explanation: A Cartesian coordinate system is a coordinate system that specifies each point uniquely in a plane by a pair of numerical coordinates.

---

101.Which join types are there in a join condition:
a) Cross join
b) Natural join
c) Join with USING clause
d) All of the mentioned

Answer: d
Explanation: INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN, EQUIJOIN are the types of joins.

---

102.How many join conditions are there?
a) 2
b) 3
c) 4
d) 5

Answer: d
Explanation: INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN, EQUIJOIN.

---

103.A condition is referred to as __________
a) Join in SQL
b) Join condition
c) Join in SQL & Condition
d) None of the mentioned

Answer: b
Explanation: An SQL join clause combines records from two or more tables in a database. It creates a set that can be saved as a table or used as it is. A JOIN is a means for combining fields from two tables by using values common to each.

---
   
   
   

