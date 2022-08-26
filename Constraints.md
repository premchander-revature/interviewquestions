1.What is Constraints and why we should use it ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- In a table, a constraint is a rule that restricts the values which can be entered into it.
- When you construct it, it can be added to a table or a view. A table can be made without restrictions.
- To improve the quality and integrity of data by utilising limitations. We can make sure the data complies with the standards we have established for it. Eg. Variable pay for an employee is not null.

</blockquote>

</details>

------

2.What are the types of constraints in SQL ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

In SQL five types of constraints are there 
- <b>Primary Key Constraint</b>: It serves as a means of identifying a table's row and ensures that every row has a unique value that cannot be NULL.
- <b>Foreign Key Constraint</b>: It makes sure that the values in one column correspond to those in another table's column.
- <b>Unique Constraint</b>: It makes sure each row in the table contains a different value.
- <b>Not Null Constraint</b>: It guarantees that a value can't be NULL.
- <b>Check Constraint</b>: A certain need is met by the check restriction.

</blockquote>

</details>

------

3.How do we create a constraint?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

When introducing a constraint as a component of the CREATE statement, there are two ways to define it:
1.Inline: next to the line of the column 
2.Out of line: at the conclusion of the CREATE statement

</blockquote>

</details>

------

4.How should we name a constraints?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- You should be able to determine which table and column a constraint applies to by looking at its name.
- Constraint name having a  combination of :
    - A two letter term indicates the type of constraint.
    - Table name is abbreviated
    - an abbreviated name for the constraint's columns or rule
There would be an underscore between each of these. 
For instance, the primary key "pk employee id" refers to the column with in employee table (emp) and is a primary key (pk) (id)

</blockquote>

</details>

------


5.What is mean by primary key constraint?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- The row's identification is referred to as a primary key constraint. It must have a uniques value for the column and it cannot be NULL
- A table can have only one primary key on it. Use of a second primary key results in an error.
- It works in the combination of both Not null constraint and Unique constraint.

</blockquote>

</details>

------

6.How to create a primary key and write a syntax ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

```sql 
CONSTRAINT constraint_name PRIMARY KEY constraint_paramaters;
```

</blockquote>

</details>

------

7.What are the Primary key restrictions?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Primary key columns cannot contain any NULL values. 
- There can only be one primary key for table or view.
- Any of the following types of columns— LOB, BFILE, TIMESTAMP WITH TIME ZONE, LONG, LONG RAW, VARRAY, NESTED TABLE, REF, or a user-defined type cannot be used as the primary key columns.
- There can be no more than 32 columns in a composite primary key.
- A primary key and a nique constraint cannot be a part in the same column or the combination of columns.

</blockquote>

</details>

------

8.Can you show me a Inline Primary key example.

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
CREATE TABLE employee (employee_id NUMBER(10) PRIMARY KEY, first_name VARCHAR2(200),
  last_name VARCHAR2(200),
  salary NUMBER(10),
  hire_date DATE
);
```
</blockquote>
</details>

------

9.How can you create a Primary key on a table using the inline method and providing a name.

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)


<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql
CREATE TABLE employee (
  employee_id NUMBER(10) CONSTRAINT pk_emp_id PRIMARY KEY,
  first_name VARCHAR2(200),
  last_name VARCHAR2(200),
  salary NUMBER(10),
  hire_date DATE
);
```
<blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>
- The table is created, and a primary key constraint with the name `pk_emp_id` is created on the table.

</blockquote>
</details>
</details>

------

10.What is the way to create a constraint on a table by using out of line method ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

```sql

CREATE TABLE employee (
  employee_id NUMBER(10),
  first_name VARCHAR2(200),
  last_name VARCHAR2(200),
  salary NUMBER(10),
  hire_date DATE,
  CONSTRAINT pk_emp_id PRIMARY KEY (employee_id)
);
```
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- This method also allows you to name the primary key, which is named pk_emp_id. We specify the column name in brackets.

</blockquote>

</details>
</details>

------

11.What is the foreign key constraint and how it works ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- To connect a column(s) in one table with a primary key or unique key in another table, a foreign key constraint is used.
- A record in one table is related to a record in another table thanks to the ability to enforce referential integrity.
- Your tables should have foreign key constraints on them if you want to make sure that the quality data in your database.
- By use of foreign keys make sure you relate your data correctly.

</blockquote>

</details>

------

12.How to create a foreign key constraint ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

Similar like primary key we can create a foreign key adding the table and column.

```sql 
CONSTRAINT constraint_name PRIMARY KEY constraint_paramaters;
```
</blockquote>

</details>

------

13.What are the foreign key restrictions ?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- The following types of columns are restricted to be used in foreign keys: LOB, BFILE, TIMESTAMP WITH TIME ZONE, LONG, LONG RAW, VARRAY, NESTED TABLE, REF, or a user-defined type.
-There must already be a primary key or unique key created on the table be referenced by the foreign key.
- It cannot have more than 32 columns.
- The table contains both the primary key and unique key constraint must be on the same database.
- When using CREATE TABLE AS to create a table and using a subquery in the AS clause, a foreign key cannot be defined. To accomplish this, you should first create the table before using the ALTER TABLE statement to add one.

</blockquote>

</details>

------

14.How you determine the referenced data when you delete the parent record.

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

ON DELETE clause is the clause of a foreign key.
There are two options:
- ON DELETE SET NULL: When the parent record is deleted, all of the child records' referenced columns will be set to NULL.
- ON DELETE SET CASCADE: All of the child records will also be deleted when the parent record is also deleted.

</blockquote>

</details>

------

15.How to declare a Inline foreign key ?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

The declaration of Inline foreign key syntax below.

```sql
CREATE TABLE employee ( employee_id NUMBER(20), first_name VARCHAR(150), last_name VARCHAR(150), salary NUMBER(10), hire_date DATE, department_id NUMBER(10) CONSTRAINT fk_emp_deptid REFERENCES department(dept_id) );
```

</blockquote>

</details>

------

16.Define Unique Constraint and What is it?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- A unique constraint, which specifies the field or set of fields in a table where a certain combination must be unique.
- Every value in a column that has a unique constraint placed on it must be unique.

Syntax of Unique Constraint below:

```sql
CONSTRAINT constraint_name UNIQUE (columns)
```
</blockquote>

</details>

------

17.How unique constraint differs from primary key constraint.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- The primary key cannot include NULL Values, but a unique constraint can.
- However, a table can only have one primary key but many unique constraints.

</blockquote>

</details>

------

18.What are the restrictions having in Unique Constraint.

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Any of the following types of columns are not allowed in the unique constraint: LOB, TIMESTAMP WITH TIMEZONE, LONG, LONG RAW, VARRAY, NESTED TABLE, REF, or a user-defined type.
- There can be no more than 32 columns in a composite unique constraint.
- The primary key and unique constraint cannot share the same columns.

</blockquote>

</details>

------

19.By constraining a SQL statement, we can restrict the _______ according to specific constraints.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.Row<br>
b.Database<br>
c.Column<br>
d.Table<br>


<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>
b. Database
</blockquote>

</details>

------

20.How many types of SQL constraint ?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

a.5<br>
b.6<br>
c.2<br>
d.3<br>


<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>
c. 2
</blockquote>

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

- SQL constraints are of two types one is Table level and Column level Constraint.
</blockquote>

</details>
</details>

------

21.How column level constraint differs from table level constraint ?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

- If constraints applied in a single column is refer as column level constraints and if the constraints applied in a multiple columns is refer as table level constraints.

</blockquote>

</details>

------

22. `NULL` refers to

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.-1<br>
b.1<br>
c.Empty<br>
d.0<br>

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>
c. Empty
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- `NULL` refers to empty only not even a zero.
</blockquote>

</details>
</details>

------

23.Which integrity is acheived by using a foreign key ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.Domain Integrity<br>
b.User-defined Integrity<br>
c.Entity Integrity<br>
d.Referential Integrity<br>

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>
d. Referential Integrity
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Referential integrity means relationship between the tables. In each table must have a primary key in a database. In other words, the condition of a set of tables in which all references to another table from one table are valid.
</blockquote>

</details>
</details>

------

24.The UNIQUE constraint can be used to______the existing tables too.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.Modify<br>
b.Change<br>
c.Delete<br>
d.Drop<br>

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>
a. Modify
</blockquote>

</details>

------

25.Which of the following does not include a foreign key?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.SET NULL<br>
b.NO ACTION<br>
c.CASCADE<br>
d.None of the above<br>

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>
c.CASCADE
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- CASCADE is a built in mechanism in foreign key constraints to enforce the data integrity.

</blockquote>
</details>
</details>

------

26.Which SQL constraint must be used in order to add a value to a field that has not had one added explicitly?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a.`DEFAULT`<br>
b.`UNIQUE`<br>
c.`CHECK`<br>
d.`NOT NULL`<br>

<details>
<summary> <b>Show Answer</b> </summary>

<blockquote>

a.`DEFAULT`
</blockquote>

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- `DEFAULT` is a used to set a default value for a column.

</blockquote>
</details>
</details>

------

