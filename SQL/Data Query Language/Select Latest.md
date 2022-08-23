1. what are Data Query Language (DQL) commands?

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

The DQL statements can be used in order to query the data and information contained in schema objects. The goal of the DQL Commands is to return a schema relation on the basis of the query supplied to them.

Syntax:

```sql

SELECT expression FROM table_x WHERE code_conditions;

```

Example:

```sql

SELECT Stu_Name FROM Student WHERE Phone = 9039462908;

```

</blockquote>
<details>
<summary><b>Explanation</b></summary>
<blockquote>

The command given above would select the record from the table ‘Student’ where the phone number is ‘9039462908’.

</blockquote>
</details>
</details>

---

2. What is the purpose of `SELECT` command in SQL?

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

DQL is a portion of a SQL statement that allows you to get and organise data from a database. You can use the SELECT command to extract data from a database in order to perform actions on it. It is the same as the projection operation in relational algebra. The result of a SELECT statement on a table or collection of tables is compiled into a new temporary table, which is subsequently displayed or received by a program, i.e. a front-end.

The chosen clause, which would be the first and one of the last clauses of a select statement, is examined by the database server. The reason for this is that before we can determine what to include in the final result set, we need to know all the alternative columns that can be included.

</blockquote>
</details>

---

3. Which of the following SQL statement is valid?

```sql

a.SELECT \* FROM Employees WHERE Gender = 'F';

b.SELECT \* FROM Employees;

c.SELECT Gender= 'M' FROM Employees;

d.SELECT Gender FROM Employees WHERE Last_Name = 'Gowda';

```

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

d) SELECT Gender FROM Employees WHERE Last_Name = 'Gowda';

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

The Statement in Option d is used to Select the Gender data from the table with a where condition stating that the last name should be "Gowda" which is a valid query.

</blockquote>
</details>
</details>

---

4. Which statement is used to get all data from the student table whose name starts with p?

```SQL
a.SELECT \* FROM student WHERE name LIKE '%p%';

b.SELECT \* FROM student WHERE name LIKE '\_p%';

c.SELECT \* FROM student WHERE name LIKE 'p%';

d.SELECT \* FROM student WHERE name LIKE '%p';

```

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

```SQL
c.SELECT \* FROM student WHERE name LIKE 'p%';

```

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

The '%' symbol indicates zero or more characters next to where it will be used.

The \* symbol is used to match exactly one character. Therefore option C is the correct choice.

  </blockquote>
  </details>
  </details>

---

5. The SQL \_\_\_\_\_\_\_ clause is used to sort the data in ascending or descending order, based on one or more columns.

a.Order By

b.Group By

c.From

d.Using

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

a.Order By

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

By default ORDER BY sorts the data in ascending order.

We can use the keyword DESC to sort the data in descending order and the keyword ASC to sort in ascending order.

</blockquote>
</details>
</details>

---

6. Which keyword is employed to only return unique values?

a.DISTINCTIVE

b.DISTINCT

c.DIFFERENT

d.UNIQUE

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

b.DISTINCT

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

SELECT DISTINCT statement is used to return only distinct (different) values inside a table.

</blockquote>
</details>
</details>

---

7. In a SELECT statement querying a single table, according to the SQL-92 standard the Asterisk(\*) means that

a.All records meeting the full criteria are to be returned.

b.All columns of the table are to be returned.

c.All records with even partial criteria met are to be returned.

d.None of the above.

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

b.All columns of the table are to be returned.

</blockquote>

<details>
<summary> Explanation</summary>
<blockquote>

By title, the outcome is arranged in ascending order. All columns from the Book table should be included in the result set, as shown by the asterisk (\*) in the select list.

</blockquote>
</details>
</details>

---

8. Each set of duplicable rows is only selected once using the distinct command.

a.SELECT DIFFERENT

b.SELECT UNIQUE

c.SELECT DISTINCT

d.All of the above

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

c.SELECT DISTINCT

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

Because of a column (or columns) on a table, the distinct command is used to choose only one duplicate of each group of duplicable rows.

</blockquote>
</details>
</details>

---

9. Which of the SQL Statements is correct syntax for SELECT Command?

a.SELECT Username, Password FROM Users.

b.SELECT Username AND Password FROM Users.

c.SELECT Username, Password WHERE Username = "User1".

d.None of the above.

<details>
<summary><b>Show Answer</b></details>
<blockquote>

a.SELECT Username, Password FROM Users.

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

```SQL
           The Correct order of SELECT Command is , FROM and WHERE clause:
                         SELECT column_name1, column_name2, ....
                          FROM table_name
                          WHERE condition
        So, only
              SELECT Username, Password FROM Users

```

follows the above syntax.

<blockquote> 
</details>
</details>
                       
---
10. A Subquery in an SELECT statement is enclosed in:

a.CAPITAL LETTERS

b.Square Brackets[]

c.Parenthesis ()

d.CURLY BRACES{}

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

c.Parenthesis ()

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

Unless there are many columns in the main query so that the subquery can compare its selected columns, a subquery can only have one column in the SELECT clause.

</blockquote>
</details>
</details>

---

11. Which of the following is a data query statement in QUEL?

a.RETRIEVE

b.GET

c.SELECT

d.None of the above.

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

c.SELECT

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

It is used to define the table columns on which the index is to be produced as well as the name of the secondary index that will be created. Index on table "name" is "name" ([column-name], [column-name,...]) A table, index, or view may be deleted using it.

</blockquote>
</details>
</details>

---

12. When two or more \_\_\_\_\_ statements are used, the UNION operator merges the results.

a.INSERT

b.UPDATE

c.DELETE

d.SELECT

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

d.SELECT

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

With the Union operator, you may aggregate the output of two or more queries into a single result set that contains every row that was returned by every Union-related query. In layman's terms, it combines the duplicate rows from two or more row sets.

</blockquote>
</details>
</details>

---

13. Which is the correct syntax for UNION Operator?

a.SELECT column_name(s) FROM TABLE table_name1
UNION
SELECT column_name(s) FROM TABLE table_name2

b.SELECT column_name(s) FROM table_name1
UNION
SELECT column_name(s) FROM table_name2

c.SELECT column_name(s) FROM table_name1
UNION table_name2

d.SELECT column_name(s) FROM table_name1 UNION table_name2

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

b.SELECT column_name(s) FROM table_name1
UNION
SELECT column_name(s) FROM table_name2

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

SELECT column_name(s) FROM table_name1 UNION SELECT column_name(s) FROM table_name2 correct syntax for applying UNION operator.

</blockquote>
</details>
</details>

---

14. Following the completion of a transaction, it must be executed to save all the operations performed in the transaction. Here we are talking about which command?

a.REVOKE

b.COMMIT

c.ROLLBACK

d.SAVE

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

b.COMMIT

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

Following the completion of a transaction, the COMMIT command must be executed to save all the operations performed in the transaction.

</blockquote>
</details>
</details>

---

15. Table Employee has 10 Records. It has a non - NULL SALARY column which is also UNIQUE. The SQL statement

```sql
SELECT COUNT(*) FROM Employee WHERE SALARY > ANY (SELECT SALARY FROM EMPLOYEE);
```

Prints

a.10

b.5

c.9

d.0

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

b.5

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

Each non-NULL value in the SALARY column of the employee table's 10 records is distinct, i.e. different. As a result, out of those ten records, one must be a minimum and cannot exceed any of the nine values in the pay column. So, nine times will the condition WHERE SALARY > ANY (SELECT SALARY FROM employee) be true. The COUNT(\*) returns 9.

</blockquote>
</details>
</details>

---

16. Which of the following query finds the names of the sailors who have reserved atleast one boat?

a.SELECT DISTINCT s.name FROM sailors , reserves WHERE s.sid = r.sid;

b.SELECT s.sname FROM sailors s ,reservers r WHERE s.sid = r.sid;

c.SELECT DISTINCT s.name FROM sailors s, reserves r WHERE s.sid = r.sid;

d.None of these

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

c.SELECT DISTINCT s.name FROM sailors s, reserves r WHERE s.sid = r.sid;

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

Using the `SELECT` query and the SQL `DISTINCT` keyword, all duplicate records are removed, leaving just the unique records in the database.

</blockquote>
</details>
</details>

---

17. Debug the SQL query?

```SQL

SELECT Id, name, YEAR(BillingDate) AS Year
FROM Records
WHERE Year >= 2010

```

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

```SQL

    SELECT Id, name, YEAR(BillingDate) AS Year
    FROM Records
    WHERE Year(BillingDate) >= 2010;

```

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

    The expression BillingYear in the WHERE clause is invalid. Even though it is defined as an alias in the SELECT phrase, which appears before the WHERE phrase, the logical processing order of the phrases of the statement is different from the written order.

</blockquote>
</details>
</details>

---

18. Debug the Error for the given SQL query?

```SQL

SELECT id, name
FROM students
WHERE grades =
             (SELECT MAX(grades)
              FROM students
              GROUP BY subject_id);

```

<details>
<summary><b>Show Answer</b></summary>

<blockquote>

```SQL

        SELECT MARKS, COUNT (DISTINCT STUDENT_ID)
        FROM STUDENT
        GROUP BY MARKS
        HAVING MARKS > (SELECT AVG(MARKS)
                   FROM STUDENT
                   WHERE ADDRESS = ’NOIDA’ );
```

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

    In the above query we use GROUP BY MARKS means it cluster the rows with same Marks and we also use SELECT MARKS, COUNT(DISTINCT STUDENT_ID) which prints the Marks of each cluster and the count of rows of respective clusters.

</blockquote>
</details>
</details>

---

19. Predict the output for the given query.

    | ID  | NAME      | AGE | ADDRESS        | SALARY |
    | --- | --------- | --- | -------------- | ------ |
    | 1   | Ramesh    | 43  | Chennai        | 25000  |
    | 2   | Lokesh    | 25  | Delhi          | 15000  |
    | 3   | Renuka    | 23  | Kota           | 20000  |
    | 4   | Chaitanya | 25  | Mumbai         | 65000  |
    | 5   | Harish    | 27  | Karnataka      | 85000  |
    | 6   | Keerthana | 22  | Madhya Pradesh | 45000  |
    | 7   | Manju     | 24  | Kerala         | 10000  |

```SQL

SELECT \* FROM CUSTOMERS
ORDER BY NAME;

```

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

The result in an ascending order by the NAME .

| ID  | NAME      | AGE | ADDRESS        | SALARY |
| --- | --------- | --- | -------------- | ------ |
| 4   | Chaitanya | 25  | Mumbai         | 65000  |
| 5   | Harish    | 27  | Karnataka      | 85000  |
| 6   | Keerthana | 22  | Madhya Pradesh | 45000  |
| 2   | Lokesh    | 25  | Delhi          | 15000  |
| 7   | Manju     | 24  | Kerala         | 10000  |
| 1   | Ramesh    | 43  | Chennai        | 25000  |
| 3   | Renuka    | 23  | Kota           | 20000  |

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

`ORDER BY` is the command used to order a column based on our preference. By default it'll arrange in Ascending order.

</blockquote>
</details>
</details>

---

20. What will be the output for the following table by using COUNT and SUM Command?

```SQL

create table customers(customer_name varchar(20),customer_id int, phone_no text,cust_age int);

insert into customers values
("Pooja",2875,9447765123,34),
("Amrutha",2434,9834567832,28),
("Balaji",2364,8776452001,56),
("Sarath",8627,9900544732,78),
("Ajith",6766,6905478823,22);

SELECT COUNT(customer_id), customer_name FROM Customer GROUP BY customer_name;
select*from customers;

The Syntax for SUM Command:

SELECT COUNT(colname) FROM table name;

SELECT SUM(customer_id)FROM customers WHERE cust_age< 30;

```

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

The Output for COUNT Command will be,

| customer_id | customer_name |
| ----------- | ------------- |
| 1           | Pooja         |
| 1           | Amrutha       |
| 1           | Balaji        |
| 1           | Sarath        |
| 1           | Ajith         |

The Output for SUM Command will be,

| Sum(customer_id) |
| ---------------- |
| 2900             |

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

The COUNT() function returns the number of rows that matches a specified criterion and The SUM() function returns the total sum of a numeric column.

</blockquote>
</details>
</details>
---

21. Predict the output:

Given the following tables

Table 1: worker

| Id  | name             |
| --- | ---------------- |
| 1   | Guillermo Sparks |
| 2   | Gene Roberts     |
| 3   | Ally Jones       |
| 4   | Bryant Summers   |
| 5   | Candice Green    |

Table 2: departments

| id  | name      | manager_id |
| --- | --------- | ---------- |
| 1   | Financial | 3          |
| 2   | Strategy  | 5          |
| 3   | IT        | 1          |
| 4   | Marketing | NULL       |

What will be the result of the query below?

```SQL

SELECT name
FROM worker
WHERE id NOT IN (SELECT manager_id FROM departments)

```

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

| name           |
| -------------- |
| Gene Roberts   |
| Bryant Summers |

</blockquote> 
<details>
<summary><b>Explanation</b></summary>
<blockquote>

</blockquote> 
</details>
</details>

---

22. How to select UNIQUE records from a table using a SQL Query?

|Table: Employees|

| EMPLOYEE_ID | NAME     | SALARY |
| ----------- | -------- | ------ |
| 100         | Jennifer | 4400   |
| 100         | Jennifer | 4400   |
| 101         | Michael  | 13000  |
| 101         | Michael  | 13000  |
| 101         | Michael  | 13000  |
| 102         | Pat      | 6000   |
| 102         | Pat      | 6000   |
| 103         | Den      | 11000  |

<details>

<summary><b>Show Answer</b></summary>

<blockquote>

Query:

```sql

  SELECT EMPLOYEE_ID,
  NAME,
  SALARY
  FROM EMPLOYEE
  GROUP BY EMPLOYEE_ID, NAME, SALARY;

```

Result:

| EMPLOYEE_ID | NAME     | SALARY |
| ----------- | -------- | ------ |
| 100         | Jennifer | 4400   |
| 101         | Michael  | 13000  |
| 102         | Pat      | 6000   |
| 103         | Den      | 11000  |

</blockquote>
</details>

---

23. Write the sql query to get the employee details using last name ?

|Table: Employees|

| First_Name | Last_Name | Birth_Date  | Gender | Joining_Date |
| ---------- | --------- | ----------- | ------ | ------------ |
| Ajay       | Kumar     | Mar-15-1970 | M      | Apr-05-2017  |
| David      | Richard   | Feb-17-1985 | M      | Mar-05-2017  |
| Junaid     | M         | Sep-28-1987 | M      | Mar-09-2016  |
| Janvi      | Gowda     | Oct-22-1993 | F      | Apr-09-2015  |
| Shobika    | Kumar     | Aug-22-1996 | F      | Apr-15-2014  |

a.SELECT \* FROM Users WHERE Gender = 'F';

b.SELECT \* WHERE Gender = 'M' FROM Employees;

c.SELECT Gender= 'M' FROM Employees;

d.SELECT Gender FROM Employees WHERE Last_Name = 'Kumar';

<details>

<summary> <b>Show Answer</b> </summary>

<blockquote>

d) SELECT Gender FROM Employees WHERE Last_Name = 'Kumar';

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

By using SELECT key in addition to WHERE clause to be used for Last_Name

</blockquote> 
</details>
</details>

---

24. Write a SQL query to find salespeople who receive commissions between 0.12 and 0.14 (begin and end values are included). Return salesman_id, name, city, and commission.

|Sales|

| salesman_id | name           | city       | commission |
| ----------- | -------------- | ---------- | ---------- |
| 5001        | James Goosling | Chennai    | 0.15       |
| 5002        | Andrews        | Pallavaram | 0.13       |
| 5005        | Pit Bull       | London     | 0.11       |
| 5006        | Mc Donalds     | Porur      | 0.14       |
| 5007        | Paul Walker    | Rome       | 0.13       |
| 5003        | Lakshaya       | Saints Row | 0.12       |

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

```SQL

SELECT \*
FROM Sales
WHERE commission BETWEEN 0.12 AND 0.14;

```

</blockquote>
<details>
<summary><b>Explanation</b></summary>
<blockquote>

we are required to select everything from the table salesman, where commission is between 0.12 and 0.14.
For this we will be using WHERE and BETWEEN commands to accquire the same.

</blockquote> 
</details>
</details>

---

25. Create a query to get the most recent table record?

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

```sql

create table Student(Student_ID int, Stu_Name varchar(20), Stu_Subject_ID text, Stu_Marks int, Stu_Age int);

insert into student values(101, "Bharathi", Bsc102, 75, 21);
insert into student values(102, "Sandhiya", BE104, 89, 20);
insert into student values(103, "Pooja", Bsc102, 43, 20);
insert into student values(104, "Vinoth", Bsc102, 56, 21);
insert into student values(107, "Shreemathi", BCA103, 98, 22);

Syntax to find the first record from the table:

SELECT * FROM Table_Name WHERE Rowid = SELECT MAX(Rowid) from Table_Name;

```

Using the aforementioned technique, we can quickly locate the last row of any table.

The following query shows the last row of the student table in the output:

```SQL

SELECT * FROM Student WHERE Rowid = SELECT MAX(Rowid) from Student;

```

Output:

| Student_ID | Stu_Name   | Stu_Subject_ID | Stu_Marks | Stu_Age |
| ---------- | ---------- | -------------- | --------- | ------- |
| 107        | Shreemathi | BCA103         | 98        | 22      |

</blockquote>
<details>
<summary><b>Explanation</b></summary>
<blockquote>
 
We have used the select command to select and see the maximum of Rowid of that table.

</blockquote> 
</details>
</details>

---

26. Write a query in SQL to retrieve only an odd number of rows from the table?

<details>
<summary> Show Answer </summary>
<blockquote>

```SQL

create table Student(Student_ID int, Stu_Name varchar(20), Stu_Subject_ID text, Stu_Marks int, Stu_Age int);


insert into student values(101, "Bharathi", Bsc102, 75, 21);
insert into student values(102, "Sandhiya", BE104, 89, 20);
insert into student values(103, "Pooja", Bsc102, 43, 20);
insert into student values(104, "Vinoth", Bsc102, 56, 21);
insert into student values(107, "Shreemathi", BCA103, 98, 22);

```

Syntax to find the Odd number of rows from the table:

```SQL

SELECT * FROM Table_Name WHERE MOD (Rowid,2) = 1 ;

```

We can easily retrieve the odd rows from the table by using the MOD function in the WHERE clause of the SELECT statement.

The following query shows odd rows of Student table in the result:

```SQL
SELECT * FROM Student WHERE MOD (Rowid,2) = 1 ;

```

Output:

| Student_ID | Stu_Name   | Stu_Subject_ID | Stu_Marks | Stu_Age |
| ---------- | ---------- | -------------- | --------- | ------- |
| 101        | Bharathi   | Bsc102         | 75        | 21      |
| 103        | Pooja      | Bsc102         | 43        | 20      |
| 107        | Shreemathi | BCA103         | 98        | 22      |

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>
 
We have used the select command to see the odd number of rows in a table by using MOD functions.
</blockquote> 
</details>
</details>

---

27. Write an SQL query to fetch the Stu_Name and Stu_Marks of those students whose age is 20.

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

```SQL

SELECT Stu_Name, Stu_Marks FROM Student WHERE Stu_Age = 20;

```

Output:

| Stu_Name | Stu_Marks |
| -------- | --------- |
| Sandhiya | 89        |
| Pooja    | 43        |

</blockquote>
<details>
<summary><b>Explanation</b></summary>
<blockquote>

We have to use the WHERE clause in the SELECT statement.

</blockquote> 
</details>
</details>

---

28.Write a query to show the maximum marks of each subject.

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

```SQL
Select Student_ID, Stu_Subject_ID, MAX(Stu_Marks) from Student group by Stu_Subject_ID;

```

Output:

| Student_ID | Stu_Subject_ID | MAX(Stu_Marks) |
| ---------- | -------------- | -------------- |
| 101        | Bsc102         | 75             |
| 102        | BE104          | 89             |
| 107        | BCA103         | 98             |

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

We need to use the MAX function with the GROUP BY statement.

 </blockquote>
 </details>
 </details>

---

29. Write a query to show all the record of those students whose Marks is greater than 82 and age is 22

<details>
<summary> Show Answer </summary>
<blockquote>

```SQL

SELECT * FROM Student WHERE Stu_Marks > 82 and Stu_Age = 22;

```

Output:

| Student_ID | Stu_Name   | Stu_Subject_ID | Stu_Marks | Stu_Age |
| ---------- | ---------- | -------------- | --------- | ------- |
| 107        | Shreemathi | BCA103         | 98        | 22      |

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

Here, we have to use the AND operator between the two conditions in the WHERE clause. The AND operator returns those records which match the specified conditions.

</blockquote>
</details>
</details>

---

30. Write a query in structured query language to view all student details from the Student table order by Stu_ID Descending.

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

```SQL

SELECT * FROM Student ORDER BY Stu_ID DESC;
```

Output:

| Student_ID | Stu_Name   | Stu_Subject_ID | Stu_Marks | Stu_Age | Stu_Address |
| ---------- | ---------- | -------------- | --------- | ------- | ----------- |
| 107        | Shreemathi | BCA103         | 98        | 22      | NULL        |
| 104        | Vinoth     | Bsc102         | 56        | 21      | NULL        |
| 103        | Pooja      | Bsc102         | 43        | 20      | NULL        |
| 102        | Sandhiya   | BE104          | 89        | 20      | NULL        |
| 101        | Bharathi   | Bsc102         | 75        | 21      | NULL        |

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

Here, we have to use the ORDER BY clause, which shows the student details in the descending order of Stu_ID.

</blockquote>
</details>
</details>

---

31. Write a Query in SQL to show the first N characters of the string column from the Student table.

<details>
<summary><b>Show Answer</b></summary>

```SQL

SELECT SUBSTRING(Column_Name, 1, N) from Table_Name;

```

This syntax uses the SUBSTRING function, which shows the specific characters of the string.

Example:

The following query shows the first two characters of Stu_Name from the Student table:

Output:
SELECT SUBSTRING(Stu_Name, 1, 2) from Student;

| SUBSTRING(Stu_Name, 1, 2) |
| ------------------------- |
| Bh                        |
| Sa                        |
| Po                        |
| Vi                        |
| Sh                        |

</blockquote>
</details>

---

32. Write a query in SQL to fetch the values of the Stu_Name column from the Student table in the upper case.
<details>
<summary><b>Show Answer</b></summary>
<blockquote>

```SQL

SELECT UPPER(column_name)from table_name;
The following syntax of uppercase as follows,
         SELECT UPPER(Stu_Name) from Student;


```

Output:

| UPPER(Stu_Name) |
| --------------- |
| BHARATHI        |
| SANDHIYA        |
| POOJA           |
| VINOTH          |
| SHREEMATHI      |

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

The following query use the UPPER function with that column name whose values are to be shown in upper case.

</blockquote>
</details>
</details>

---

33. Write a query to show the record of those students whose name begins with the 's' character.

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

```SQL
        SELECT * FROM table_name WHERE column_name LIKE '%s';
The following syntax of uppercase as follows,
        SELECT * FROM Student WHERE Stu_Name LIKE '%s';

```

Output:

| Student_ID | Stu_Name   | Stu_Subject_ID | Stu_Marks | Stu_Age | Stu_Address |
| ---------- | ---------- | -------------- | --------- | ------- | ----------- |
| 102        | Sandhiya   | BE104          | 89        | 20      | NULL        |
| 107        | Shreemathi | BCA103         | 98        | 22      | NULL        |

<details>
<summary>Explanation</summary>
<blockquote>

The following query we have to use the LIKE operator, which matches the given pattern in the table.

</blockquote>
</details>
</details>

---

34. Table-Runners

| id  | name          |
| --- | ------------- |
| 1   | John Dave     |
| 2   | Jane Smith    |
| 3   | Alice Fox     |
| 4   | Bobby Lashley |
| 5   | Lisa jack     |

Table-Races

| id  | event         | winner_id |
| --- | ------------- | --------- |
| 1   | 100 meter     | 2         |
| 2   | 500 meter     | 3         |
| 3   | Cross-Country | 2         |
| 4   | Marathon      | NULL      |

What will be the result of the query below?

```sql
SELECT \* FROM Runners WHERE id NOT IN (SELECT winner_id FROM Races);

```

<details>
<summary>Show Answer</summary>
<blockquote>

| id  | name          |
| --- | ------------- |
| 1   | John Dave     |
| 4   | Bobby Lashley |
| 5   | Lisa jack     |

</blockquote>

---

35. Given two tables created and populated as follows:

```SQL

CREATE TABLE dbo.data(id int, user_id int);
CREATE TABLE dbo.documents(ID int, Pages int, Text varchar(100));

INSERT INTO dbo.data VALUES
(1,1),
(2,2),
(3,3);

INSERT INTO dbo.documents(ID,Pages) VALUES
(1,5),
(2,6),
(null,0);

What will the result be from the following query:



UPDATE docs SET Text=Pages FROM docs INNER JOIN data ON data.id=documents.ID;
WHERE EXISTS (
SELECT 1 FROM dbo.documents
WHERE ID=data.id
);

```

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

| idnum  | pageseq | doctext  |
| ------ | ------- | -------- |
| 1      | 5       | 5        |
| 2      | 6       | 6        |
| NULL   | 0       | NULL     |

</blockquote>
</details>

---

36. Assume a schema of Employee ( Id, Name, Department_Id ) , DEPT ( Id, Name).

If there are 20 records in the Employee table and 10 records in the DEPT table, how many rows will be displayed in the result of the following SQL query:
Select \* From Employee, DEPT

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

The query will result in 200 rows as a “cartesian product” or “cross join”, which is the default whenever the ‘where’ clause is omitted.

</blockquote>
</details>
</details>

---

37. Given two tables created as follows

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

Write a query to fetch values in table Sample_a that are and not in Sample_b without using the NOT keyword.

<details>
<summary><b>Show Answer</b></summary>

<blockquote>

select _ from Sample_a
except
select _ from Sample_b;

</blockquote>
</details>

---

38. How to organise the patients in descending order and sort them according to the fees they are being assessed.

TABLE : HOSPITAL

| No   | Name     | Age  | Department        | Datofadm | Charges | Sex |
| ---- | -------- | ---- | ----------------- | -------- | ------- | --- |
| 1    | Sandeep  | 65   | Surgery           | 23/02/98 | 300     | M   |
| 2    | Ravina   | 24   | Orthopedic        | 20/01/98 | 200     | F   |
| 3    | Karan    | 45   | Orthopedic        | 19/02/98 | 200     | M   |
| 4    | Tarun    | 12   | Surgery           | 01/01/98 | 300     | M   |
| 5    | Zubin    | 36   | ENT               | 12/02/98 | 250     | M   |
| 6    | Ketaki   | 16   | ENT               | 24/02/98 | 300     | F   |
| 7    | Ankita   | 29   | Cardiology        | 20/02/98 | 800     | F   |
| 8    | Zareen   | 45   | Gynecology        | 22/02/98 | 300     | F   |
| 9    | Kush     | 19   | Cardiology        | 13/01/98 | 800     | M   |
| 10   | Shaliya  | 31   | Nuclear Medicine  | 19/02/98 | 400     | M   |

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

```SQL


SELECT Name from HOSPITAL GROUP BY Charges ORDER BY DESC;

```

</blockquote>

<details>
<summary><b>Explanation</b></summary>
<blockquote>

According to the Question We are asked to Sort the patient based on their Name in Desc order and group it based the fees they are being charged.

so we will first Select The Name column from the Hospital Table and moving on we arange them in desc order using

</blockquote>
</details>
</details>

---

39. Table – Worker

| WORKER_ID | FIRST_NAME | LAST_NAME | SALARY | JOINING_DATE        | DEPARTMENT |
| --------- | ---------- | --------- | ------ | ------------------- | ---------- |
| 001       | Monika     | Arora     | 100000 | 2014-02-20 09:00:00 | HR         |
| 002       | Niharika   | Verma     | 80000  | 2014-06-11 09:00:00 | Admin      |
| 003       | Vishal     | Singhal   | 300000 | 2014-02-20 09:00:00 | HR         |
| 004       | Amitabh    | Singh     | 500000 | 2014-02-20 09:00:00 | Admin      |
| 005       | Vivek      | Bhati     | 500000 | 2014-06-11 09:00:00 | Admin      |
| 006       | Vipul      | Diwan     | 200000 | 2014-06-11 09:00:00 | Account    |
| 007       | Satish     | Kumar     | 75000  | 2014-01-20 09:00:00 | Account    |
| 008       | Gopika     | Chauhan   | 90000  | 2014-04-11 09:00:00 | Admin      |

i) What is the query to find the position of the alphabet (‘g’) in the first name column ‘Gopika’ from Worker table.

ii) What is the way for fetching the unique values of DEPARTMENT from Worker table and printing its length.

iii) Write an SQL query to print all Worker details from the Worker table order by FIRST_NAME in Ascending order and DEPARTMENT in Descending order.

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

i)

```sql
Select INSTR(FIRST_NAME, BINARY'g') from Worker where FIRST_NAME = 'Gopika';
```

ii)

```sql
Select distinct length(DEPARTMENT) from Worker;
```

iii)

```sql
Select * from Worker order by FIRST_NAME asc,DEPARTMENT desc;
```

</blockquote>
</details>

---

40. Table – Worker

| WORKER_ID | FIRST_NAME | LAST_NAME | SALARY | JOINING_DATE        | DEPARTMENT |
| --------- | ---------- | --------- | ------ | ------------------- | ---------- |
| 001       | Monika     | Arora     | 100000 | 2014-02-20 09:00:00 | HR         |
| 002       | Niharika   | Verma     | 80000  | 2014-06-11 09:00:00 | Admin      |
| 003       | Vishal     | Singhal   | 300000 | 2014-02-20 09:00:00 | HR         |
| 004       | Amitabh    | Singh     | 500000 | 2014-02-20 09:00:00 | Admin      |
| 005       | Vivek      | Bhati     | 500000 | 2014-06-11 09:00:00 | Admin      |
| 006       | Vipul      | Diwan     | 200000 | 2014-06-11 09:00:00 | Account    |
| 007       | Satish     | Kumar     | 75000  | 2014-01-20 09:00:00 | Account    |
| 008       | Gopika     | Chauhan   | 90000  | 2014-04-11 09:00:00 | Admin      |

Table - Title

| WORKER_REF_ID | WORKER_TITLE  | AFFECTED_FROM       |
| ------------- | ------------- | ------------------- |
| 1             | Manager       | 2016-02-20 00:00:00 |
| 2             | Executive     | 2016-06-11 00:00:00 |
| 8             | Executive     | 2016-06-11 00:00:00 |
| 5             | Manager       | 2016-06-11 00:00:00 |
| 4             | Asst. Manager | 2016-06-11 00:00:00 |
| 7             | Executive     | 2016-06-11 00:00:00 |
| 6             | Lead          | 2016-06-11 00:00:00 |
| 3             | Lead          | 2016-06-11 00:00:00 |

i) Write an SQL query to print details of the Workers who are also Managers.

ii) Write an SQL query to fetch duplicate records having matching data in some fields of a table.

iii) Write an SQL query to show records from one table that another table does not have.

iv) Write an SQL query to show the top 5 records of the Title table.

v) How to write a SQL query to determine the 3rd highest salary in the Worker Table.

vi) Write an SQL query to fetch the list of employees with the same salary.

vii) Write an SQL query to show the second highest salary from a table.

viii) Write an SQL query to show one row twice in results from a table.

ix) Write an SQL query to fetch intersecting records of two tables.

x) How to Write an SQL query that fetches the departments that have less than five people in it.

xi) Write an SQL query to print the name of employees having the highest salary in each department.

xii) How to write an SQL query to fetch three min salaries from a table.

xiii) Write an SQL query to fetch departments along with the total salaries paid for each of them.

<details>
<summary><b>Show Answer</b></summary>

i)

```sql
SELECT DISTINCT W.FIRST_NAME, T.WORKER_TITLE

FROM Worker W

INNER JOIN Title T

ON W.WORKER_ID = T.WORKER_REF_ID

AND T.WORKER_TITLE in ('Manager');
```

ii)

```sql
SELECT WORKER*TITLE, AFFECTED_FROM, COUNT(*)

FROM Title

GROUP BY WORKER*TITLE, AFFECTED_FROM

HAVING COUNT(*) > 1;
```

iii)

```sql
SELECT _ FROM Worker

MINUS

SELECT _ FROM Title;
```

iv)

```sql
SELECT \* FROM Title ORDER BY Salary DESC LIMIT 5;
```

v)

```sql
SELECT Salary FROM Worker ORDER BY Salary DESC LIMIT 2,1;
```

vi)

```sql
Select distinct W.WORKER_ID, W.FIRST_NAME, W.Salary

from Worker W, Worker W1

where W.Salary = W1.Salary

and W.WORKER_ID != W1.WORKER_ID;
```

vii)

```sql
Select max(Salary) from Worker

where Salary not in (Select max(Salary) from Worker);
```

viii)

```sql
select FIRST_NAME, DEPARTMENT from worker W where W.DEPARTMENT='HR'

union all

select FIRST_NAME, DEPARTMENT from Worker W1 where W1.DEPARTMENT='HR';
```

ix)

```sql
(SELECT _ FROM Worker)

INTERSECT

(SELECT _ FROM WorkerClone);
```

x)

```sql
SELECT DEPARTMENT, COUNT(WORKER_ID) as 'Number of Workers' FROM Worker GROUP BY DEPARTMENT HAVING COUNT(WORKER_ID) < 5;
```

xi)

```sql
SELECT t.DEPARTMENT,t.FIRST_NAME,t.Salary from(SELECT max(Salary) as TotalSalary,DEPARTMENT from Worker group by DEPARTMENT) as TempNew

Inner Join Worker t on TempNew.DEPARTMENT=t.DEPARTMENT

and TempNew.TotalSalary=t.Salary;
```

xii)

```sql
SELECT distinct Salary from worker a WHERE 3 >= (SELECT count(distinct Salary) from worker b WHERE a.Salary >= b.Salary) order by a.Salary desc;
```

xiii)

```sql
SELECT DEPARTMENT, sum(Salary) from worker group by DEPARTMENT;
```

---
