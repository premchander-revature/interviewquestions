1. Which of the following is/are transaction control commands in SQL?

- a) Commit
- b) Rollback
- c) Both A. and B.
- d) None of the above

<details>

<summary> Show Answer </summary>

Answer:

C) Both A. and B.

Explanation:

Commit and Rollback are transaction control commands in SQL.

</details>

2. What is the Command used to Store some data's Permanently in a database.

- a) SavePoint
- b) Grant
- c) Commit
- d) All of The Above.

<details>

<summary> Show Answer </summary>

Answer:

c) Commit

Explanation:

Commit is the command used in SQL to store data permanently in a table.

</details>

3. Larry was updating a SQL table during his practical exam during which he mistakenly added few mismatched data's his examination time is about to end
   Suggest a quick solution through which he can score full marks.

- a)Revoke
- b)Grant
- c)Alter
- d)Rollback

<details>

<summary> Show Answer </summary>

Answer:

d) Rollback

Explanation:
Rollback is the command used in mySQL to restore any unsaved data in a table.

</details>

4. Few Students Mark has been uploaded in a database , to prevent the data loss from the database which command can be used

| Name          | Marks |
| ------------- | ----- |
| Addam Warlock | 67    |
| Demos         | 65    |
| Brayan        | 84    |
| Chester       | 88    |
| Duke          | 99    |

- a) Grant
- b) Select
- c) Commit
- d) Rollback

<details>

<summary> Show Answer </summary>

c) Commit

Explanation:
Commit is the command used in mySQL to store data permanently in a table.

</details>

5. Find the Error in the Following Command:
   Insert into TableExample( col1 [datatype],col2 [datatype],col3[datatype])
   values(val1,val2,val3);
   commit;
   rollback;

<details>

<summary> Show Answer </summary>

Answer:

rollback command is not applicable if a Commit is used, it is used to store data permanently in a table.

Explanation:

Commit command is used to store a data in the table permanently, therefore once the Commit command is being executed there is no way for Rollback.

</details>

6. Larry and Weasly was assigned a project in SQL they both worked seperatly hence they had some duplicate data , both are confused in finding a way to get rid of the duplicate data,Luckily Larry used a savepoint command during data insertion.
   Suggest them a solution.

- a) By using just Rollback command.
- b) By Using Only Savepoint Command
- c) Duplicate datas cant be stored in a database
- d) By Combining Savepoint and Rollback command

<details>
 
<summary> show Answer </summary>

Show Answer:

d) By Combining Savepoint and Rollback command

Explanation:

Savepoint is a command in MySQL that is like a Restore Point in Windows i.e., If an error occurs it rollbacks to the point where the restore point was created, Likewise in MySQL if we want to go to a point we will be using the
ROLLBACK TO [SAVEPOINT NAME];

</details>

7. INSERT INTO class VALUES(2, 'Rashid');

COMMIT;

UPDATE class SET name = 'Albert' WHERE id = '2';

SAVEPOINT A;

INSERT INTO class VALUES(3, 'Charlie');

SAVEPOINT B;

INSERT INTO class VALUES(4, 'Brandon');

SAVEPOINT C;

SELECT \* FROM class;

What will be the Output for the following command?

<details>

<summary> Show Answer </summary>

Answer:

| id  | name    |
| --- | ------- |
| 2   | Albert  |
| 3   | Charlie |
| 4   | Brandon |

Explanation:
The Above commands is inserting values into a table class.
and commit command is used to make sure that the data is stored permanently.
Then the is being modified using Update Command.
Savepoint is used to save that data at the certain point of time.
and the select command is used to view the data in the table.

</details>

8. What does the following code snippet do?

DELETE FROM STUDENTS
WHERE AGE = 16;
ROLLBACK;

- a) Performs an undo operation on the delete operation.
- b) Deletes the rows from the table where AGE = 16.
- c) Deletes the entire table.
- d) none of the Above.

<details>

<summary> Show Answer </summary>

Answer:
a) Performs an undo operation on the delete operation.

Explanation:
Delete Command is used to delete data from the table where age =16.
Then the data is beinged rollbacked using rollback command.

</details>

9. During transaction before commit which of the following statements is done automatically in case of shutdown?

- a) Rollback
- b) Commit
- c) View
- d) Flashback

<details>

<summary> Show Answer </summary>
 Answer:

a) Rollback

Explanation:

In case of a shutdown, before committing, Rollback is done.

</details>

10. We want to update the location of Amritha to "Gujarat" in the table “EMPLOYEE” an make sure to save the chages permanently. EMPLOYEE table is as follows:

| EMP_ID | EMP_NAME | EMP_LOC |
| ------ | -------- | ------- |
| 100    | Amritha  | Punjab  |
| 200    | Rajesh   | Mumbai  |
| 300    | Rashmika | Chennai |

<details>
<summary> Show Answer </summary>

Answer:
UPDATE EMPLOYEE SET EMP_LOC = 'Gujarat' WHERE EMP_NAME= 'Amritha';
COMMIT;

Explanation:
Update Command is used to alter the data in the table, Commit command is used to save the changes permanently.

</details>

11. Fill in the missing command based on the output,

CREATE TABLE Players(
ID INT,
First_Name VARCHAR(255),
Last_Name VARCHAR(255),
Date_Of_Birth date,
Place_Of_Birth VARCHAR(255),
Country VARCHAR(255),
PRIMARY KEY (ID)
);

insert into Players values(1, 'Jonathan', 'Swift', DATE('1981-04-22'), 'CapeTown', 'SouthAfrica');<br>
insert into Players values(2, 'Kumara', 'Sangakkara', DATE('1977-10-27'), 'Matale', 'Srilanka'); <br>
insert into Players values(1, 'Mahendra Singh', 'Dhoni', DATE('1981-07-07'), 'Ranchi', 'India');<br>

O/P:

| ID  | First_Name     | Last_Name | Date_Of_Birth | Place_Of_Birth | Country |
| --- | -------------- | --------- | ------------- | -------------- | ------- |
| 1   | Mahendra Singh | Dhoni     | 1981-07-07    | Ranchi         | India   |

<details>
<summary> Show Answer </summary>
Answer:

Rollback

Explanation:

Based on the output we can see that the insertion of the first 2 columns has been removed, Only the insertion below the missing command hence the missing command is Rollback.

</details>

12. When Working with a huge data sets, which is a smarter way to define commit command?

- a) Define commit after each insertion / Updation in the table.
- b) Defining Set Autocommit=1 at the beginning of the file.
- c) It is Not possible to save changes permanently in MySQL.
- d) The Changes are saved Permanently by Default.

<details>
<summary>Show Answer</summary>
Answer:

b)Defining Set Autocommit=1 at the beginning of the file.

Explanation:

Set Autocommit=1 is a command in MySQL that is used to enable autocommit therefore each changes stored permanently by default.

</details>

13. What is the use of SAVEPOINT command from Transition Control Language.

- a) Used to Load a file.
- b) Used to update the file in the databsase.
- c) Used to save the changes till a certain point in time.
- d) None of the Above.

<details>
<summary>Show Answer</summary>
Answer:

c) Used to save the changes till a certain point in time.

Explanation:

it is a point in a transaction when you can roll the transaction back to a certain point without rolling back the entire transaction.

</details>

<!--   9/8/22  ----->

14. In order to start the transaction, the command used is –

- a. Mysql > START COMMIT;
- b. Mysql > START TRANSACTION;
- c. Mysql > START ROLLBACK;
- d. None of the above
<details>
<summary>Show Answer</summary>

Answer:

b) Mysql > START TRANSACTION;

Explanation:

To start the transaction, Mysql > START TRANSACTION; command is used.

</details>

15. What type of join is needed when you wish to include rows that do not have matching values?

- A. Equi-join
- B. Natural join
- C. Outer join
- D. All of the above

<details>

<summary>Show Answer</summary>

Answer:

C. Outer join

Explanation:

Outer joins are joins that return matched values and unmatched values from either or both tables

</details>

16. Which is the best way to reduce the data redundancy in a database.?

- a. De-Normalization

- b. Normalization

- c. Abnormalization

- d. None of these Option

<details>

<summary>Show Answer</summary>

Answer

b. Normalization

Explanation

Normalization is the process of organizing data in a database.

</details>

17. What distinguishes constraints at the column and table levels?

- a. Constraints are applied to a single row using Column Level Constraints whereas Multiple rows can be constrained using a Table Level Constraint.
- b. Constraints are applied to multiple rows using Column Level Constraints whereas a single row can be constrained using a Table Level Constraint.
- c. Constraints are applied to a single column using Column Level Constraints whereas Multiple columns can be constrained using a Table Level Constraint.
- d. Constraints are applied to multiple columns using Column Level Constraints whereas only a single column can be constrained using a Table Level Constraint.

<details>
<summary>Show Answer</summary>

Answer:
c. Constraints are applied to a single column using Column Level Constraints whereas Multiple columns can be constrained using a Table Level Constraint

Explanation:

Constraints are applied to a single column using Column Level Constraints whereas Multiple columns can be constrained using a Table Level Constraint.

</details>

18. Regarding the NOT NULL Constraint, which is considered TRUE among the following?

- a. In columns that are subject to the NOT NULL constraint, duplicate values are not allowed.
- b. When a table's column is declared as NOT NULL, no record in the table can have an empty value for that column.
- c. By applying the NOT NULL constraint, we will always ensure that the column contains a unique value and won't allow nulls.
- d. The value will first be checked for certain conditions before inserting it into the column when a NOT NULL constraint applies to a column in the table.

<details>
<summary>Show Answer</summary>

B. When a table's column is declared as NOT NULL, no record in the table can have an empty value for that column

Explanation:

When a table's column is declared as NOT NULL, no record in the table can have an empty value for that column.

</details>

19. \***\*\_\_\_\*\*** and \***\*\_\_\*\***constraints form the core of the PRIMARY KEY constraint.

- a. NOT NULL , CHECK
- b. NOT NULL , DEFAULT
- c. NOT NULL , FOREIGN KEY
- d. NOT NULL , UNIQUE
<details>
<summary>Show Answer</summary>

Answer:

d. NOT NULL , UNIQUE

Explanation:

NOT NULL and UNIQUE constraints form the core of the PRIMARY KEY constraint.

</details>

20. A foreign key is utilised to achieve \_\_\_\_\_\_ integrity.

- a. Referential Integrity
- b. Domain Integrity
- c. User-defined Integrity
- d. Entity Integrity
<details>
<summary>Show Answer</summary>

Answer:

a. Referential Integrity

Explanation:

Referential integrity is a constraint applied on foreign, which requires the foreign key to have a matching primary key or provided primary key is not a null value

</details>

21. Regarding the DEFAULT Constraint, which is considered TRUE among the following?

- a. The value will first be checked for certain conditions before inserting it into the column when a DEFAULT constraint applies to a column in the table.
- b. In the event of a DEFAULT constraint being applied to a table's column without a user specifying the value to be inserted when that constraint was applied, the default value that was specified when the constraint was applied will be put into that column.
- c. An index can be created on the table using the DEFAULT constraint.
- d. None of the above
<details>
<summary>Show Answer</summary>
Answer:

b) In the event of a DEFAULT constraint being applied to a table's column without a user specifying the value to be inserted when that constraint was applied, the default value that was specified when the constraint was applied will be put into that column

Explanation:

In the event of a default constraint is applied to a table's column without a user specifying the value to be inserted when that constraint was applied, the default value that was specified when the constraint was applied will be put into that column.

</details>

22. Which of the following is TRUE about SQL Concatenate?

- a. It is also possible to combine more than two strings into one string.
- b. Two columns of the table may be used to store the strings that are to be combined, or they may just be stored individually without being stored into the table.
- c. When the concatenated strings are stored in separate columns of a table, they are stored in the column in which they were initially stored.
- d. All of the above
<details>
<summary>Show Answer</summary>

Answer:

d. All of the above

Explanation:

In case of SQL Concatenate:

more than two strings may be combined into a single string.
The strings that need to be merged can either be put in two columns of the table or they can be saved separately without being stored in the table.When the concatenated.
Strings are kept separate in a table's columns; they are kept in the column where they were kept initially.

</details>

23. You may obtain the date data using the \_\_\_ function in a more legible format.

- a. DATE
- b. DATE_FORM
- c. DATE_FORMAT
- d. DATE_VALUE

<details>
<summary>Show request</summary>

Answer:

c. DATE_FORMAT

Explanation:

DATE_FORMAT function is the best way to retrieve the date in a more formal way, such that it will be easy to understand.

</details>

24. Which clause makes use of the BETWEEN operator?

- a. IF
- b. EXCEPT
- c. WHERE
- d. AS

<details>
<summary>Show Answer</summary>
Answer: C) WHERE

Explanation:

In WHERE clause, BETWEEN operator is used.

</details>

25. In CRUD Operator, U is an acronym of –

- a. Upper
- b. Unique
- c. Update
- d. Uppercase
<details>
<summary>Show Answer</summary>

Answer:

c. Update

Explanation:

U in CRUD Operator refers to Update.

</details>

26. What does the Read in CRUD Operator mean?

- a. To retrieve data
- b. To fetch data
- c. Both A. and B.
- d. None of the above
<details>
<summary>Show Answer</summary>

Answer:

c. Both A. and B.

Explanation:

Read in CRUD Operator means to retrieve and fetch the data from the table.

</details>

27. Using the DELETE Query from the CRUD Operator, we can delete

- a. Only one row
- b. All the rows
- c. Only two rows
- d. None of the above
<details>
<summary>Show Answer</summary>

Answer:

b. All the rows

Explanation:

Using the DELETE Query from the CRUD Operator, we can delete all the rows from the table.

</details>

28. The sub query must be used before \_\_\_\_ in order to avoid duplicate records being returned by the sub query.

- a. Many Value Operators
- b. Multiple Value Operators
- c. Single Value Operator
- d. Unique Value Operator
<details>
<summary>Show Answer</summary>

Answer:

b. Multiple Value Operators

Explanation:

In order to prevent multiple records from being returned by the sub query, multiple value operators must be used before the sub query.

</details>

29. An SQL \_\_\_ is a virtual table whose contents are determined by the outcomes of the SQL statement.

- a. Concatenate
- b. Virtual
- c. View
- d. None of the above
<details>
<summary>Show Answer</summary>
Answer:

c. View

Explanation:

An SQL View is a virtual table, whose contents are based on the SQL statement's results.

</details>

30. What is TRUE about UPDATE in SQL VIEW?

- a. Views that depend on a single table can be updated.
- b. An update of a view created from more than one table will not be allowed by SQL.
- c. There should be no NULL values in the fields of view.
- d. All of the above
<details>
<sumamry>Show Answer</summary>

Answer:

d. All of the above

Explanation:

UPDATE in SQL VIEW states that-

i) Views that depend on a single table can be updated.
ii) An update of a view created from more than one table will not be allowed by SQL.
iii) There should be no NULL values in the fields of view.

</details>

31. Which statement is TRUE about the HAVING Clause?

- a. In order to group the rows, HAVING Clause is used.
- b. In order to return the rows, HAVING Clause is used.
- c. In order to select the defined groups by the GROUP BY Clause, HAVING Clause is used.
- d. None of the above
<details>
<sumamry>Show Answer</summary>

Answer:

c. In order to select the defined groups by the GROUP BY Clause, HAVING Clause is used

Explanation:

In order to select the defined groups by the GROUP BY Clause, HAVING Clause is used.

</details>

32. Find the Student_Name whose Dept is CSE OR Branch is CS using SQL query:

Table; Details

| Student_ID | Student_Name | Dept   | Branch Course |
| ---------- | ------------ | ------ | ------------- |
| 100        | Aman Praveen | MBBS   | MBBS          |
| 101        | Abin Devasy  | CSE CS | B.Sc          |
| 102        | Keerthy      | CSE CS | B.Sc          |
| 103        | Praveen      | MBA    | HR operations |

<details>
<summary>Show Answer</summary>

Answer:

SELECT Student_Name from Details WHERE Dept="CSE CS";

Explanation:

We are Asked to Select the Student Who are from CSE CS Department, therefore we will be using SELECT and WHERE Clauses to get the desired output.

</details>

33. In the section relation which of the following is used as a foreign key?

a) Course_id

b) Course_id,sec_id

c) Room_number

d) Course_id,sec_id,room_number

<details>
<summary> Show Answer </summary>

Answer: a

</details>

34. In order to include an attribute Name to the teaches relation which of the following command is used?

a) Alter table teaches include Name;

b) Alter table teaches add Name;

c) Alter table teaches add Name varchar;

d) Alter table teaches add Name varchar(20);

<details>
<summary> Show Answer </summary>

Answer: d

</details>

35. To replace the relation section with some other relation the initial step to be carried out is

a) Delete section;

b) Drop section;

c) Delete from section;

d) Replace section new_table ;

<details>
<summary> Show Answer </summary>

Answer: b

</details>

36. Which of the following command is used to display the departments of the instructor relation?

a) Select \* from instructor where Dept_name = Finance;

b) Select \* from instructor ;

c) Select dept_name from instructor;

d) Select dept_name for instructor where Name=Jackson;

<details>
<summary> Show Answer </summary>

Answer: c

</details>

37. How can we select the elements which have common Dept_name in both the relation ?

a) Select \* from instructor i , course c where i.Dept_name=c.Dept_name;

b) Select Dept name from instructor ,Course ;

c) Select \* from instructor i , course c ;

d) Select Dept_name from instructor where Dept_name = NULL;

<details>
<summary> Show Answer </summary>

Answer: a

</details>

38. If a person all the people in Music department gets fired which of the following has to be performed on the instructor relation?

a) Delete Dept_name=Music in instructor;

b) Delete from instructor where Dept_name=Music;

c) Remove Dept_name= Music

d) All of the mentioned

<details>
<summary> Show Answer </summary>

Answer: b

</details>

39. Which function is used to find the count of distinct departments?

a) Dist

b) Distinct

c) Count

d) Count,Dist

<details>
<summary> Show Answer </summary>

Answer: a

</details>

40. Which function is used to identify the title with Least scope?

a) Min(Credits)

b) Max(Credits)

c) Min(title)

d) Min(Salary)

<details>
<summary> Show Answer </summary>

Answer: a

</details>

41. A domain is ******\_\_\_****** if elements of the domain are considered to be indivisible units.

a) Atomic

b) Subatomic

c) Substructure

d) Subset

<details>
<summary> Show Answer </summary>

Answer: a

</details>

42. Identify the composite attributes

a) Salary

b) Credits

c) Section_id

d) None of the mentioned

<details>
<summary> Show Answer </summary>

Answer: d

</details>

43. Which one is based on multi-valued dependency:

a) First

b) Second

c) Third

d) Fourth

<details>
<summary> Show Answer </summary>

Answer: d

</details>

44. If a relation is in BCNF, then it is also in

a) 1 NF

b) 2 NF

c) 3 NF

d) All of the mentioned

<details>
<summary> Show Answer </summary>

Answer: d

</details>

45. If every non-key attribute is functionally dependent primary key, then the relation will be in

a) First normal form

b) Second normal form

c) Third form

d) Fourth normal form

<details>
<summary> Show Answer </summary>

Answer: b

</details>

46. If an attribute of a composite key is dependent on an attribute of the other composite key, a normalization called **\_** is needed.

a) DKNF

b) BCNF

c) Fourth

d) Third

<details>
<summary> Show Answer </summary>

Answer: b

</details>

47. The term for information that describes what type of data is available in a database is:

a) Data dictionary

b) data repository

c) Index data

d) Metadata

<details>
<summary> Show Answer </summary>

Answer: d

</details>

48. A data type that creates unique numbers for key columns in Microsoft Access is:

a) Autonumber

b) Boolean

c) Sequential key

d) Sequential number

<details>
<summary> Show Answer </summary>

Answer: a

</details>

49. A dependency exist between two columns when

a) Together they constitute a composite key for the table

b) Knowing the value in one column determines the value stored in another column

c) The table is in 3NF

d) Together they constitute a foreign key

<details>
<summary> Show Answer </summary>

Answer: a

</details>

50. In the ******\_\_****** normal form, a composite attribute is converted to individual attributes.

a) First

b) Second

c) Third

d) Fourth

<details>
<summary> Show Answer </summary>

Answer: a

</details>

51. Tables in second normal form (2NF):

a) Eliminate all hidden dependencies

b) Eliminate the possibility of a insertion anomalies

c) Have a composite key

d) Have all non key fields depend on the whole primary key

<details>
<summary> Show Answer </summary>

Answer: a

</details>

52. Key to represent relationship between tables is called

a) Primary key

b) Secondary Key

c) Foreign Key

d) None of the mentioned

<details>
<summary> Show Answer </summary>

Answer: c

</details>
