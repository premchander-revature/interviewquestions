1.What is an Operator in SQL?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary>
<blockquote>

An operator is a reserved word or a character which is  used as primarily in an SQL statement's WHERE clause to perform operations, like comparisons and arithmetic operations.

</blockquote>
</details>

2.What are the types of Operators used in SQL?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary>
<blockquote>

Generally, there are 3 types of operators in SQL.
* Arithmetic Operators.
* Comparison Operators.
* Logical Operators.

</blockquote>
</details>

3.What are the types of relational operators?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary>
<blockquote>

There are 6 types of Relational Operators and they are,

|    Operators  |           Operations                |
|---------------|-------------------------------------|
|       <       |            less than                |
|       <=      |      less than or equal to          |
|       >       |            greater than             |
|       >=      |      greater than or equal to       |
|       ==      |             equal to                |
|       /=      |           not equal to              | 



</blockquote>
</details>

4.What is the use of special operator and their types in SQL?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary>
<blockquote>

* Special Operator are used to either increase or decrease the value of the variable one by one. Special operators. &, *, sizeof( ) and ternary operators.
* The different types of  special operators used in SQL are:
   * ALL operator
   * ANY Operator
   * BETWEEN Operator
   * EXISTS Operator
   * IN Operator
   * LIKE Operator

</blockquote>
</details>

5.what is the use of LIKE  operator in sql


![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary>
<blockquote>

* The Like is a logical operator which is used to determine whether a specific character string matches a specified pattern.
* It is commonly used in a Where clause which is used to search for a specified pattern in a column in this operator it can be useful in cases when we need to perform pattern matching instead of equal or not equal.
</blockquote>
</details>

6.Which of the following describe SQL's types for Unicode character strings?

a. ntext

b. nchar

c. Both A and B

d. None of the above.


![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

Both A and B

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

Unicode character strings datatypes in SQL includes 'nchar' and 'ntext'.

</blockquote>

</details>
</details>

7.which of the following is the best datatype to use and to store a string with up to 255 characters?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

a. BLOB

b. Binary

c. Text

d. Tiny Text

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

Tiny Text

</blockquote>

<details>  
<summary><b> Explantion </b></summary>

<blockquote>

A string in "TINY TEXT" can be up to 255 characters or 255 bytes long.

</blockquote>

</details>
</details>

8.How many Primary keys that a table have in SQL?

a. Depends on DBA

b. Only 1

c. Only 2

d. Depends on no of Columns

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

Only 1

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>
 
The fields that uniquely identify the each entry in a database can be used as the primary key alone or in combination. 

It cannot be empty or null. 

Although a table may contain multiple columns, there can only be one primary key per table.

</blockquote>

</details>
</details>

9.When is the WHERE clause used with a wildcard?

a. An exact match is necessary for a CREATE statement.

b. An exact match is necessary for a SELECT statement.

c. An exact match is not possible for a SELECT statement.

d. None of the above.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

An exact match is not possible for a `SELECT` statement.

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

When an exact match in a `SELECT` statement is not possible,  wildcard is used in the `WHERE` clause.

</blockquote>

</details>
</details>

10.Primary keys can be_______________.
a. NULL.

b. NOT NULL.

c. Both A and B.

d. Depends upon their situation.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

NOT NULL

</blockquote>

<details>
<summary><b>  Explanation  </b></summary>

<blockquote>
 
The primary key must never be empty(NOT NULL).

</blockquote>

</details>
</details>

11.Suppose if we have a database named of 'students' library details as well. The library table has 3 columns namely student ID, Name, Books. The student ID as the name suggests stored the unique student IDs. The Name column contains the names of the students. The Books column contains also the number of books acquired by the student.

| ID 	|   Name  	| Books 	|
|-------|-----------|-----------|
| 1  	| Aman    	| 7     	|
| 2  	| Sushant 	| 8     	|
| 3  	| Saumya  	| 8     	|
| 4  	| Kausiki 	| 3     	|
| 5  	| Aditya  	| 6     	|

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

So there are some set of operations by using set operators.

```sql

SELECT * FROM student WHERE Name LIKE 'S%'
UNION
SELECT * FROM library WHERE Books >= 7

```

Output:

| ID 	|   Name  	| Books 	|
|-------|-----------|-----------|
| 1  	| Aman    	| 7     	|
| 2  	| Sushant 	| 8     	|
| 3  	| Saumya  	| 8     	|

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

In this query, we have the output of both the queries merged as a single output Hence, we will get the details of the students whose name starts with 'S' as well as the library details of the students who have acquired more than 7 books.

</blockquote>

</details>
</details>

12.In this example, we have a table called "suppliers" with the following data:

| supplier_id 	| supplier_name     	| city             	| state      	|
|-------------	|-------------------	|------------------	|------------	|
| 100         	| Microsoft         	| Redmond          	| Washington 	|
| 200         	| Google            	| Mountain View    	| California 	|
| 300         	| Oracle            	| Redwood City     	| California 	|
| 400         	| Kimberly-Clark    	| Irving           	| Texas      	|
| 500         	| Tyson Foods       	| Springdale       	| Arkansas   	|
| 600         	| SC Johnson        	| Racine           	| Wisconsin  	|
| 700         	| Dole Food Company 	| Westlake Village 	| California 	|
| 800         	| Flowers Foods     	| Thomasville      	| Georgia    	|
| 900         	| Electronic Arts   	| Redwood City     	| California 	|

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

Output:

```sql

SELECT *
FROM suppliers
WHERE supplier_name = 'Microsoft';

```

There will be 1 record selected. 
These are the results that you should see:

| supplier_id 	| supplier_name 	| city    	| state      	|
|-------------	|---------------	|---------	|------------	|
| 100         	| Microsoft     	| Redmond 	| Washington 	|

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

In this example, the `SELECT` statement above would return all rows from the suppliers table where the supplier_name is equal to Microsoft.

</blockquote>

</details>
</details>

13.The IN condition can be used with any data type in SQL. Let's look at how to use the IN condition with character (string) values.

In this example, the table name is suppliers with the following data:

| supplier_id 	| supplier_name     	| city             	| state      	|
|-------------	|-------------------	|------------------	|------------	|
| 100         	| Microsoft         	| Redmond          	| Washington 	|
| 200         	| Google            	| Mountain View    	| California 	|
| 300         	| Oracle            	| Redwood City     	| California 	|
| 400         	| Kimberly-Clark    	| Irving           	| Texas      	|
| 500         	| Tyson Foods       	| Springdale       	| Arkansas   	|
| 600         	| SC Johnson        	| Racine           	| Wisconsin  	|
| 700         	| Dole Food Company 	| Westlake Village 	| California 	|
| 800         	| Flowers Foods     	| Thomasville      	| Georgia    	|
| 900         	| Electronic Arts   	| Redwood City     	| California 	|

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

Output:

```sql

SELECT *
FROM suppliers
WHERE supplier_name IN ('Microsoft', 'Oracle', 'Flowers Foods');

```

There will be 3 records selected. These are the results that you should see:

| supplier_id 	| supplier_name 	| city         	| state      	|
|-------------	|---------------	|--------------	|------------	|
| 100         	| Microsoft     	| Redmond      	| Washington 	|
| 300         	| Oracle        	| Redwood City 	| California 	|
| 800         	| Flowers Foods 	| Thomasville  	| Georgia    	|

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

This example would return all rows from the suppliers table where the supplier_name is either Microsoft, Oracle or Flowers Foods Because the * is used in the select, all fields from the suppliers table would appear in the result set. 

using the `IN` condition makes the statement easier to read and more efficient than using multiple `OR` conditions.

</blockquote>

</details>
</details>

14. What will be the main difference between ‘BETWEEN’ and ‘IN’ condition operators?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>


The Example of using  `BETWEEN` Operator:

```sql

SELECT * FROM Students where ROLL_NO BETWEEN 10 AND 50;

```

The Example of using `IN` Operator:

```sql

SELECT * FROM students where ROLL_NO IN (8,15,25);

```

<details>
<summary><b>  Explanation  </b></summary>

<blockquote>

`BETWEEN` operator is used to display rows based on a range of values in a row.

the `IN` condition operator is used to check for values contained in a specific set of values.

</blockquote>

</details>
</details>

15.According to SQL Standard, the `SUM` operator should disregard a value of:

a. 0's

b. 1's

c. NULL value

d. String

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

NULL value

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

The `SUM()` function returns NULL, not zero, if it is used in a `SELECT` statement that returns no rows. 

The `SUM()` function is told by the `DISTINCT` parameter to only add up distinct values in a set. 

The `NULL` values are not considered in the calculation by the `SUM()` function.

</blockquote>

</details>
</details>

16. Which of the following should be used to find the mean of the salary from the below given query ? 

```sql

SELECT __________
FROM instructor
WHERE dept name= ’Comp. Sci.’;

```

a. Mean(salary)

b. Count(salary)

c. Sum(salary)

d. Avg(salary)

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

Avg(salary)

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

`Avg()` function is used to find the mean of the values.

</blockquote>

</details>
</details>

17.`TINYTEXT` can hold the maximum length of ____________ characters?

a. 254

b. 255

c. 256

d. 257

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

255

</blockquote>

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Explanation </b></summary>

<blockquote>

`INYTEXT` can hold the maximum length of 255 characters.

</blockquote>

</details>
</details>

18.Which data type can store unstructured data in a column?

a. CHAR

b. RAW

c. NUMERIC

d. VARCHAR

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote> 

RAW

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

The term `Raw` refers to a form of data type that may hold unstructured data in a column pattern. 

Binary data is stored using this type of data type.

Since this data cannot be changed, it is referred to as unstructured data. 

Instead, it can only be inserted or queried. 

Additionally, this raw data type could contain bytes of huge sizes.

</blockquote>

</details>
</details>

19.What distinguishes a SQL Server `HAVING CLAUSE` from a `WHERE CLAUSE`?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote> 

HAVING Clause:

Only the `SELECT` statement is used with the `HAVING CLAUSE` and It is typically used in a query's `GROUP BY` clause also.

`HAVING` functions as a `WHERE` clause in the absence of `GROUP BY`.
 The aggregate function supports the `HAVING clause`.

```sql

Syntax:

SELECT expr1, expr2, expr3..,  
FROM tables  
WHERE condition   
GROUP BY expr1, expr2, expr3..,  
HAVING condition; 

```

WHERE Clause:

Before a row is included in a query  `GROUP BY` function, the `WHERE` clause is applied to it  and  the aggregate function cannot be used with the `WHERE` clause.

```sql

Syntax:

`WHERE` condition;  

```

</blockquote> 

</details>

20.Consider we have an employees table with the following data:

| E_ID 	|        Name       	| Salary 	| City       	| Designation        	| Date_of_Joining 	| Age 	|
|-------|-----------------------|-----------|---------------|-----------------------|-------------------|-------|
| 1    	| Sakshi Kumari     	| 50000  	| Mumbai     	| Project Manager    	| 2021-06-20      	| 24  	|
| 2    	| Tejaswini Naik    	| 75000  	| Delhi      	| System Engineer    	| 2019-12-24      	| 23  	|
| 3    	| Anuja Sharma      	| 40000  	| Jaipur     	| Manager            	| 2021-08-15      	| 26  	|
| 4    	| Anushka Tripathi  	| 90000  	| Mumbai     	| Software Tester    	| 2021-06-13      	| 24  	|
| 5    	| Rucha Jagtap      	| 45000  	| Bangalore  	| Project Manager    	| 2020-08-09      	| 23  	|
| 6    	| Rutuja Deshmukh   	| 60000  	| Bangalore  	| Manager            	| 2019-07-17      	| 26  	|
| 7    	| Swara Baviskar    	| 55000  	| Jaipur     	| System Engineer    	| 2021-10-10      	| 24  	|
| 8    	| Sana Sheik        	| 45000  	| Pune       	| Software Engineer  	| 2020-09-10      	| 26  	|
| 9    	| Swati Kumari      	| 50000  	| Pune       	| Software Tester    	| 2021-01-01      	| 25  	|
| 10   	| Mayuri Patel      	| 60000  	| Mumbai     	| Project Manager    	| 2020-10-02      	| 24  	|
| 11   	| Simran Khanna     	| 45500  	| Kolhapur   	| HR                 	| 2019-01-02      	| 26  	|
| 12   	| Shivani Wagh      	| 50500  	| Delhi      	| Software Developer 	| 2016-09-10      	| 25  	|
| 13   	| Kiran Maheshwari  	| 50000  	| Pune      	| HR                 	| 2013-12-12      	| 23  	|
| 14   	| Tejal Jain        	| 40000  	| Delhi      	| Project Manager    	| 2017-11-10      	| 25  	|
| 15   	| Mohini Shah       	| 38000  	| Pune       	| Software Developer 	| 2019-03-05      	| 20  	|


20.Write a query to retrieve only those records of employees from the employees table where the designation is'Project Manager' and the City to which the employee belongs to is Mumbai.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote> 

Query:

```sql

SELECT * FROM employees WHERE City = "Mumbai" AND Designation = "Project Manager";  

```

Output:

| E_ID 	|      Name     	| Salary 	| City   	| Designation     	| Date_of_Joining 	| Age 	|
|-------|-------------------|-----------|-----------|-------------------|-------------------|-------|
| 1    	| Sakshi Kumari 	| 50000  	| Mumbai 	| Project Manager 	| 2021-06-20      	| 24  	|
| 10   	| Mayuri Patel  	| 60000  	| Mumbai 	| Project Manager 	| 2020-10-02      	| 24  	|

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote> 

There are only two records in the employees table whose city name is equal to 'Mumbai' and designation name is equal to 'Project Manager'.

a `SELECT` query using the `AND` operator between the two requirements and a WHERE clause on the City and Designation columns. if there is any entry in , the employee belongs to Mumbai and has the title of project manager—will only be taken into account for determining output.

</blockquote>

</details>
</details>

21.Write a query to retrieve only those records of an employee from the employees table where employee salary lies between 50000 to 80000.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

Query:

```sql

SELECT * FROM employees WHERE Salary BETWEEN 50000 AND 80000;  

```

So, We have the following Output given below:

| E_ID 	|        Name       	| Salary 	| City      	| Designation        	| Date_of_Joining 	| Age 	|
|------ |-----------------------|-----------|---------------|-----------------------|-------------------|-------|
| 1    	| Sakshi Kumari     	| 50000  	| Mumbai    	| Project Manager    	| 2021-06-20      	| 24  	|
| 2    	| Tejaswini Naik    	| 75000  	| Delhi     	| System Engineer    	| 2019-12-24      	| 23  	|
| 3    	| Anuja Sharma      	| 40000  	| Jaipur     	| Manager            	| 2021-08-15      	| 26  	|
| 5    	| Rucha Jagtap      	| 45000  	| Bangalore  	| Project Manager    	| 2020-08-09      	| 23  	|
| 6    	| Rutuja Deshmukh   	| 60000  	| Bangalore 	| Manager            	| 2019-07-17      	| 26  	|
| 7    	| Swara Baviskar    	| 55000  	| Jaipur    	| System Engineer    	| 2021-10-10      	| 24  	|
| 8    	| Sana Sheik        	| 45000  	| Pune       	| Software Engineer  	| 2020-09-10      	| 26  	|
| 9    	| Swati Kumari      	| 50000  	| Pune      	| Software Tester    	| 2021-01-01      	| 25  	|
| 10   	| Mayuri Patel      	| 60000  	| Mumbai    	| Project Manager    	| 2020-10-02      	| 24  	|
| 11   	| Simran Khanna     	| 45500  	| Kolhapur   	| HR                 	| 2019-01-02      	| 26  	|
| 12   	| Shivani Wagh      	| 50500  	| Delhi     	| Software Developer 	| 2016-09-10      	| 25  	|
| 13   	| Kiran Maheshwari  	| 50000  	| Pune      	| HR                 	| 2013-12-12      	| 23  	|
| 14   	| Tejal Jain        	| 40000  	| Delhi      	| Project Manager    	| 2017-11-10      	| 25  	|
| 15   	| Mohini Shah       	| 38000  	| Pune       	| Software Developer 	| 2019-03-05      	| 20  	|

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

In the above query we have used the `BETWEEN` operator to create a `SELECT` query on the Salary column with a `WHERE` clause. Beginning and end values of 50000 and 80000, respectively, are placed after the `BETWEEN` operator, with the `AND` operator coming after each.

</blockquote>

</details>
</details>

22.Write a query to retrieve only those records of employees from the employees table where the employee's designation is 'System Engineer' or the city to which the employee belongs is Mumbai.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

Query:

```sql

SELECT * FROM employees WHERE Designation = "System Engineer" OR City = "Mumbai";

```

The Following Output will be,

| E_ID 	|        Name       	| Salary 	| City   	| Designation     	| Date_of_Joining 	| Age 	|
|-------|-----------------------|-----------|-----------|-------------------|-------------------|-------|
| 1    	| Sakshi Kumari     	| 50000  	| Mumbai 	| Project Manager 	| 2021-06-20      	| 24  	|
| 2    	| Tejaswini Naik    	| 75000  	| Delhi  	| System Engineer 	| 2019-12-24      	| 23  	|
| 4    	| Anushka Tripathi  	| 90000  	| Mumbai 	| Software Tester 	| 2021-06-13      	| 24  	|
| 7    	| Swara Baviskar    	| 55000  	| Jaipur 	| System Engineer 	| 2021-10-10      	| 24  	|
| 10   	| Mayuri Patel      	| 60000  	| Mumbai 	| Project Manager 	| 2020-10-02      	| 24  	|

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

Here, the `OR` operator has already been placed between the two requirements in a `SELECT` query with a `WHERE` clause on the City and Classification columns. such as the employee's home city is Mumbai or their job title is System Engineer.

</blockquote>

</details>
</details>

23.Write a query to retrieve only those records of employees from the employees table where the city to which the employee belongs to is either Mumbai, Bangalore, or Pune.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

Query:

```sql

SELECT * FROM employees WHERE City IN ("Mumbai", "Bangalore", "Pune");  

```

| E_ID 	|        Name       	| Salary 	| City       	| Designation        	| Date_of_Joining 	| Age 	|
|:----:	|:-----------------:	|--------	|------------	|--------------------	|-----------------	|-----	|
| 1    	| Sakshi Kumari     	| 50000  	| Mumbai     	| Project Manager    	| 2021-06-20      	| 24  	|
| 4    	| Anushka Tripathi  	| 90000  	| Mumbai     	| Software Tester    	| 2021-06-13      	| 24  	|
| 5    	| Rucha Jagtap      	| 45000  	| Bangalore  	| Project Manager    	| 2020-08-09      	| 23  	|
| 6    	| Rutuja Deshmukh   	| 60000  	| Bangalore  	| Manager            	| 2019-07-17      	| 26  	|
| 8    	| Sana Sheik        	| 45000  	| Pune       	| Software Engineer  	| 2020-09-10      	| 26  	|
| 9    	| Swati Kumari      	| 50000  	| Pune       	| Software Tester    	| 2021-01-01      	| 25  	|
| 10   	| Mayuri Patel      	| 60000  	| Mumbai     	| Project Manager    	| 2020-10-02      	| 24  	|
| 15   	| Mohini Shah       	| 38000  	| Pune       	| Software Developer 	| 2019-03-05      	| 20  	|

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

In this query,  a `SELECT` query containing a `WHERE` clause on the City column and the `IN` operator has been constructed. We have given  the `IN` operator the parameters Mumbai, Bangalore, and Pune because we only wanted records that were located in Mumbai, Bangalore, or Pune. Therefore, the City value of any record will only be taken into account in the output if it matches the places supplied to the `IN` operator.

</blockquote>

</details>
</details>

24.










https://www.sanfoundry.com/database-mcqs-basic-sql-operations/




