# DBMS

1. What is DBMS?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary><b> Show Answer </b></summary>
<blockquote>

- A database management system (DBMS) is a piece of software that enables users to quickly create, define, and manipulate databases. A tool or interface is provided by DBMS so that we may carry out a variety of tasks, such as building databases, putting data in them, updating them, adding tables to them, and many other things.

- The databases are also secured and protected by DBMS. Additionally, it keeps data integrity when there are several users.
</blockquote>
</details>

---

# Database

2. What are different types of Databases?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary><b> Show Answer </b></summary>
<blockquote>

Two categories of databases exist:

- Non-Relational Database
- Relational Database

Non-relational databases: These don't use tables to arrange their data. Data is kept in key-value pairs for storage. JSON and XML are two examples of non-relational databases.

SQL cannot be used to communicate with non-relational databases.

Relational databases: Tables are used to arrange data in relational databases. Data are arranged in columns and rows in a table. Each row of the table is identified by a distinct key.

</blockquote>
</details>

---

3. Describe SQL?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary><b> Show Answer </b></summary>
<blockquote>

- SQL, or Structured Query Language, is a standardised language for communicating with relational database management systems (Relational Database Management System). Popular examples of relational databases include MySQL, Oracle, MariaDB, PostgreSQL, and others.

- C.R.U.D (Create, Retrieve, Update & Delete) operations on relational databases are carried out using SQL.

- SQL can also handle database administration duties including user management, database security, and backup.

- SQL may be used to construct databases and tables.

</blockquote>
</details>

---

4. What are the types of Sub Querys in Structured Query Language(SQL)?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary><b> Show Answer </b></summary>
<blockquote>

Structured Query Language Types (SQL)

- `DQL` (Data Query Language)
  The data that is already present in the database is fetched using DQL.`SELECT` is the DQL command.

- `DDL` (Data Definition Language)
  Table schemas are defined by DDL. `CREATE`, `DROP`, and `ALTER` are the DDL commands.

- `DCL` (Data Control Language)
  For managing users and permissions, DCL are used, Access to the database is controlled by it. The commands are `GRANT` and `REVOKE`.

- `DML` (Data Manipulation Language)
  DML is used to add, update, and remove data from databases. `INSERT`, `DELETE`, and `UPDATE` are the three DML commands.

- `TCL` (Transaction Control Language)
  Transaction management operations in the database are performed using TCL. The `COMMIT` and `ROLLBACK` TCL commands.

</blockquote>
</details>

---

5. What is `Query`?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary><b> Show Answer </b></summary>
<blockquote>

A query is a series of instructions you provide the database management system that informs it what data you want to get, add, update, or remove from the database.

</blockquote>
</details>

---

6. Name some popular SQL Vendors.

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<sumamry><b>Show Answer</b></summary>

<blockquote>

The top 5 SQL Vendors are:

- Microsoft SQL
- MYSql
- ORACLE Database 12c
- Amazon Relational Database Service (AWS RDS)
- Postgre SQL

</blockquote>

</details>

---

7. What are the common datatypes present in SQL?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

The common datatypes are:

- CHAR(n)
- VARCHAR(n)
- INT
- FLOAT
- DATE

</blockquote>

<details>

<summary><b>Explanation</b></summary>

<blockquote>

`Data type Description:`

- CHAR(n)

  Specifies character type data of length n where n could be any value from 0 to 255.

- VARCHAR(n)

  Specifies character type data of length ‘n’ where n could be any value from 0 to 65535. But unlike CHAR, VARCHAR is a variable-length data type.

  That is,declaring VARCHAR (30) means a maximum of 30 characters can be stored but the actual allocated bytes will depend on the length of entered string.

- INT
  <br>specifies an integer value. Each INT value occupies 4 bytes of storage.

  The range of values allowed in integer type are -2147483648 to 2147483647.

- FLOAT
  <br>Holds numbers with decimal points. Each FLOAT value occupies 4 bytes.

  DATE The DATE type is used for dates in 'YYYY-MM-DD' format. YYYY is the 4 digit year, MM is the 2 digit month and DD is the 2 digit date. The supported range is '1000-01-01' to '9999-12-31

</blockquote>

</details>

</details>

---

8. What exactly is a SQL constraint?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Explanation</b></summary>

<blockquote>

Constraints are certain types of restrictions on the data
values that an attribute can have. They are used to
ensure the accuracy and reliability of data.

</blockquote>

</details>

---

9. What are some of the most prevalent SQL constraints?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Some Common SQL Constraints are:

- `NOT NULL`
- `UNIQUE`
- `DEFAULT`
- `PRIMARY KEY`
- `FOREIGN KEY`

</blockquote>

<details>

<summary><b>Explanation</b></summary>

<blockquote>

- `NOT NULL`
  Ensures that a column cannot have NULL values where NULL means missing/
  unknown/not applicable value.

- `UNIQUE`
  Ensures that all the values in a column are distinct/unique.

- `DEFAULT`
  A default value specified for the column if no value is provided.

- `PRIMARY KEY`
  The column which can uniquely identify each row or record in a table.

- `FOREIGN KEY`
  The column which refers to value of an attribute defined as primary key in another table.

</blockquote>

</details>

</details>

---
