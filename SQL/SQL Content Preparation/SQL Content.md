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
