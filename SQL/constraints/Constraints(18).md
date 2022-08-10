1.What is Constraints and why we should use it ?


<details>
<summary> Show Answer </summary>

- A constraint is a rule that you defining on a table that it restricts the values in that table.
- It can be added to a table or a view when you create it. We can create a table without constraints.
- Purpose of using constraints to imporve the quality and integrity of data. We can help ensure that the data meets the rules that we have set for it. Eg. an Employee's variable pay is not null

</details>

2.What are the types of constraints in SQL ?

<details>
<summary> Show Answer </summary>

In SQL five types of constraints are there 
- <b>Primary Key Constraint</b>: It ensures all rows have a uniue value and it cannot be NULL, also used as a identifier of a table's row
- <b>Foreign Key Constraint</b>: It ensures that values in a columns match values in another tables 
column
- <b>Unique Constraint</b>: It ensure all the rows in table have a unique value.
- <b>Not Null Constraint</b>: It ensure a value cannot be NULL.
- <b>Check Constraint</b>: Check constraint meets a specific condition.

</details>

3.How do we create a constraint?

<details>
<summary> Show Answer </summary>

There are two ways to define a constraint when adding it as part of the CREATE statement
- 1.Inline : next to the line of the column 
- 2.Out of line : at the end of the CREATE statement

</details>

4.How should we name a constraints?

<details>
<summary> Show Answer </summary>

- Your constraint names should be able to be used to identify which table and column.
- Constraint name has a combination of :
    - A two letter term to indicate the type of constraint 
    - An abbreviated name of the table
    - An abbreviate name of the columns or rule for the constraint
Each of these would be separated by an underscore.
Eg: "pk_employee_id" is a primary key (pk) refers to the employee table (emp) and refers to the column (id)

</details>


5.What is mean by primary key constraint?

<details>
<summary> Show Answer </summary>

- A primary key constraint refers to identifier of a row. It must have a uniques value for the column and it cannot be NULL
- A table can only have one primary key on it. If try to use second primary key it shows an error.
- A primary key works in the combination of Not null constraint and Unique constraint.

</details>

6.How to create a primary key ?

<details>
<summary> Show Answer </summary>

```sql 
CONSTRAINT constraint_name PRIMARY KEY constraint_paramaters;
```
</details>

7.What are the Primary key restrictions?

<details>
<summary> Show Answer </summary>

- No values in primary key columns can be NULL 
- A table or view can have only one primary key
- The columns in the primary key cannot be any of the following type LOB, BFILE, TIMESTAMP WITH TIME ZONE, LONG, LONG RAW, VARRAY, NESTED TABLE, REF, or a user defined type.
- A composite primary key can't have more than 32 columns.
- The same column or the combination of columns cannot be a part of primary key and a unique constraint.

</details>

8.Can you show me a Inline Primary key example.

<details>
<summary> Show Answer </summary>

```sql
CREATE TABLE employee (employee_id NUMBER(10) PRIMARY KEY, first_name VARCHAR2(200),
  last_name VARCHAR2(200),
  salary NUMBER(10),
  hire_date DATE
);
```
</details>

9.How can you create a Primary key on a table using the inline method and providing a name.


<details>
<summary> Show Answer </summary>

```sql

CREATE TABLE employee (
  employee_id NUMBER(10) CONSTRAINT pk_emp_id PRIMARY KEY,
  first_name VARCHAR2(200),
  last_name VARCHAR2(200),
  salary NUMBER(10),
  hire_date DATE
);

```
The table is created, and a primary key constraint with the name pk_emp_id is created on the table.

</details>

10.What is the way to create a constraint on a table by using out of line method

<details>
<summary> Show Answer </summary>

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

This method also allows you to name the primary key, which is named pk_emp_id. We specify the column name in brackets.

</details>

11.What is the foreign key constraint and how it works ?

<details>
<summary> Show Answer </summary>

- A foreign key constraint is used to create a link between a column(s) in one table and a primary key or unique key in another table.
- It allows you to enforce referential integrity, which means that a record in one table relates to a record in another table.
- If you want to ensure you have quality data in your database, your tables should have foreign key constraints on them.
- By using foreign keys ensure you relate your data correctly.

</details>

12.How to create a foreign key constraint

<details>
<summary> Show Answer </summary>

Similar like primary key we can create a foreign key adding the table and column.

```sql 
CONSTRAINT constraint_name PRIMARY KEY constraint_paramaters;
```

</details>

13.What are the foreign key restrictions ?

<details>
<summary> Show Answer </summary>

- The columns in the foreign key cannot be any of the following types: LOB, BFILE, TIMESTAMP WITH TIME ZONE, LONG, LONG RAW, VARRAY, NESTED TABLE, REF, or a user defined type.
- The primary key or unique key referenced by the foreign key must already be created on the referenced table.
- A composite foreign key can’t have more than 32 columns.
- Both tables (the table that has the primary key and the table that has the foreign key) must be on the same database.
- You can’t define a foreign key when creating a table using CREATE TABLE AS with a subquery in the AS clause. To do this, you’ll need to create the table first, then use the ALTER TABLE statement to add one.

</details>

14.How you determine the referenced data when you delete the parent record.

<details>
<summary> Show Answer </summary>

ON DELETE clause is the clause of a foreign key.
There are two options:
- ON DELETE SET NULL: When you delete the parent record, then all the child recordswill have referenced columnset to NULL
- ON DELETE SET CASCADE: When you delete the parent record then all the child records will be deleted as well.

</details>

15.How to declare a Inline foreign key.?

<details>
<summary> Show Answer </summary>

The declaration of Inline foreign key syntax below.

```sql
CREATE TABLE employee ( employee_id NUMBER(20), first_name VARCHAR(150), last_name VARCHAR(150), salary NUMBER(10), hire_date DATE, department_id NUMBER(10) CONSTRAINT fk_emp_deptid REFERENCES department(dept_id) );
```

</details>

16.Define Unique Constraint and What is it?

<details>
<summary> Show Answer </summary>

- A unique constraint is a type of constraint and it defines the field or set of fields where the combination must be unique in a table.
- If you create a unique constraint on one column, all of the values in that column must be unique.

Syntax of Unique Constraint below:

```sql
CONSTRAINT constraint_name UNIQUE (columns)
```

</details>

17.How unique constraint differs from primary key constraint.

<details>
<summary> Show Answer </summary>

- A unique constraint can contain NULL Values, but the primary key cannot.
- A table can have more than one unique constraint , but only one primary key.

</details>

18.What are the restrictions having in Unique Constraint.

<details>
<summary> Show Answer </summary>

- The columns in the unique constraint cannot be any of the following types: LOB, TIMESTAMP WITH TIMEZONE, LONG , LONG RAW, VARRAY, NESTED TABLE, REF or a user defined type.
- A composite unique constraint cant have more than 32 columns.
- You can't use the same columns for a unique constraint as a primary key.

</details>


