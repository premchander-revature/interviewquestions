1.Predict the output for the following table.

Let's take a Product table consisting of the following records and delete a single record from the given table below.

Table_Name: Product 
 

| Product_Id   |	Product_Name   |   Product_Price	|    Product_Quantity     |
|--------------|-----------------|------------------|-------------------------|
|  P101	       |      Chips	     |           20     |         20              |
|  P102	       |      Chocolates |           60	    |         40              |
|  P103	       |       Maggi	   |           75	    |          5              |
|  P104	       |       Biscuits	 |           80	    |         20              |
|  P105	       |      Namkeen	   |           40	    |         50              |

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

`DELETE` FROM Product `WHERE` Product_Id = P103 ; 

```

| Product_Id   |	Product_Name     |   Product_Price	|    Product_Quantity     |
|--------------|-------------------|------------------|-------------------------|
|  P101	       |      Chips	       |           20     |         20              |
|  P102	       |      Chocolates   |           60	    |         40              |
|  P104	       |       Biscuits	   |           80	    |         20              |
|  P105	       |      Namkeen	     |           40	    |         50              |

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

To delete a particular row by using the delete command. The Syntax for deleting a row is ,
         
```sql

DELETE FROM Table_Name WHERE Condition ;

```

</blockquote>

</details>
</details>

------

2.Predict the output in the below table by using the employees table and increase the income of all employees by 5% in a table.

Table Name: Employees
           
         |  Emp_Id   |   Emp_Name   |   Emp_Salary  |
         |-----------|--------------|---------------|
         |   2010    |    Ankitha   |     28000     |
         |   2020    |    Kumar     |     23000     |
         |   2030    |    Diya      |     31000     |
         |   2040    |    Poornima  |     47000     |
         |   2050    |    Abinaya   |     20000     |

Increase Income of all employees by 5% in the above given table.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

 `UPDATE` Employees `SET` Emp_Salary = Emp_Salary+(Emp_Salary*5.0/100.0);

```

| Emp_Id 	| Emp_Name 	| Emp_Salary 	|
|--------	|----------	|------------	|
| 2010   	| Ankitha  	| 29400      	|
| 2020   	| Kumar    	| 24150      	|
| 2030   	| Diya     	| 32550      	|
| 2040   	| Poornima 	| 49350      	|
| 2050   	| Abinaya  	| 21000      	|

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

Here `UPDATE` command is used for updating the salary by 5% and it is also can be used for only 5% alone it can be used for updating even 10% also.

</blockquote>

</details>
</details>

------

3.Predict the output for the following given table (Update single column)
Update the column_Name and set the value to "Divya" in all the rows where Age is 20.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

UPDATE Student WHERE Age = 20 SET NAME = "Divya" ;
UPDATE Student SET NAME = "Divya" WHERE Age = 20;

```
| ROLL_NO 	| NAME   	| ADDRESS 	| PHONE       	| Age 	|
|---------	|--------	|---------	|-------------	|-----	|
| 1       	| Ram    	| Delhi   	| 987466321   	| 18  	|
| 2       	| RAMESH 	| GURGAON 	| 7010234567  	| 18  	|
| 3       	| Divya  	| Chennai 	| 6897543222  	| 20  	|
| 4       	| SURESH 	| Delhi   	| 8756340034  	| 18  	|
| 5       	| Divya  	| Rohit   	| 7786432668  	| 20  	|

<details>
<summary><b> Explanation </b></summary>

<blockquote>

```sql

  UPDATE table_name
     SET column1 = value1, column2 = value2, ...
     WHERE condition;

```
This is the correct syntax for updating the values in the given table.
</blockquote>

</details>
</details>

------

4.Predict the output of the following by using  Inner JOINS?
Table 1:

```sql

CREATE TABLE dbo.envelope(id int, user_id int);

```

```sql

INSERT INTO dbo.envelope VALUES(1,1);
INSERT INTO dbo.envelope VALUES(2,2);
INSERT INTO dbo.envelope VALUES(3,3);

```

Table 2:

```sql

CREATE TABLE dbo.docs(idnum int, pageseq int, doctext varchar(100));

```

```sql

INSERT INTO dbo.docs(idnum,pageseq) VALUES(1,5);
INSERT INTO dbo.docs(idnum,pageseq) VALUES(2,6);
INSERT INTO dbo.docs(idnum,pageseq) VALUES(null,0);

```

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

UPDATE docs SET doctext=pageseq FROM docs INNER JOIN envelope ON envelope.id=docs.idnum
WHERE EXISTS (
SELECT 1 FROM dbo.docs
WHERE id=envelope.id);

```

Output:
| idnum 	| pageseq 	| doctext 	|
|-------	|---------	|---------	|
| 1     	| 5       	| 5       	|
| 2     	| 6       	| 6       	|
| NULL  	| 0       	| NULL    	|

<details>
<summary><b> Explanation </b></summary>

<blockquote>

* The above query's `EXISTS` clause is a red herring. Given that ID is not a member of dbo.docs, it will always be true. As a result, it will mention the comparison between the envelope table and itself!

* Since the join of `NULL` will not produce a result when trying to match with any value of envelope, the idnum value of `NULL` will not be set.
</blockquote>

</details>
</details>

------

5.Predict the output of the following for the given below syntax for inserting a table.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

create table Student(Stu_Id int, Stu_Name varchar(20), Age int, Grade Varchar(5), City varchar(20));

```

```sql

INSERT INTO STUDENT(Stu_Id, Stu_Name,Age,Grade,City) VALUES(1,"Arthi",15,"B","Andhra"),
                                                           (2,"Ganga",18,"D","Bangalore"),
                                                           (3,"Madhumitha",17,"A","Delhi"),
                                                           (4,"RIYA SREE",10,"C","Kerala"),
                                                           (5,"PRIYA GANESH",20,"B","Chennai");

```

| Stu_Id 	| Stu_Name     	|  Age    	| Grade 	| City      	|
|--------	|--------------	|---------	|-------	|-----------	|
| 1      	| Arthi        	| 15      	| B     	| Andhra    	|
| 2      	| Ganga        	| 18      	| D     	| Bangalore 	|
| 3      	| Madhumitha   	| 17      	| A     	| Delhi     	|
| 4      	| Riya Sree    	| 10      	| C     	| Kerala    	|
| 5      	| Priya Ganesh 	| 20      	| B     	| Chennai   	|

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>
 
        Insert table is used for inserting the values in the given column name in the given table.
you can insert how many of records you want by using the syntax

```sql

`INSERT` INTO table_name(Column1,Column2,Column3,.......) VALUES (Value1, Value2,Value3,.....),

                                                               (Value1, Value2,Value3,.....),

                                                               (Value1, Value2,Value3,.....);

```   
</blockquote>

</details>
</details>

------

6.Predict the output of the following  for updating a single record in table?

| EmpID 	| EmpName 	| EmpEmail       	| PhoneNumber 	| City      	|
|-------	|---------	|----------------	|-------------	|-----------	|
| 1     	| Mohan   	| mohan@xyz.com  	| 9966449966  	| Delhi     	|
| 2     	| Sonia   	| sonia@abc.com  	| 9746964799  	| Mumbai    	|
| 3     	| Sanjay  	| sanjay@pqr.com 	| 9654323456  	| Bengaluru 	|
| 4     	| Avni    	| avni@xyz.com   	| 9876543678  	| Mumbai    	|
| 5     	| Rahul   	| rahul@abc.com  	| 9542456786  	| Delhi     	|

Update Single Record:
         a query to update the 3rd employee (Employee ID) with a new phone number and city.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

UPDATE Employees
SET PhoneNumber = "9646879876", City= "Kolkata"
WHERE EmpID = 2;

```

Output:

| EmpID 	| EmpName 	| EmpEmail       	| PhoneNumber 	| City      	|
|-------	|---------	|----------------	|-------------	|-----------	|
| 1     	| Mohan   	| mohan@xyz.com  	| 9966449966  	| Delhi     	|
| 2     	| Sonia   	| sonia@abc.com  	| 9746964799  	| Kolakta    	|
| 3     	| Sanjay  	| sanjay@pqr.com 	| 9654323456  	| Bengaluru 	|
| 4     	| Avni    	| avni@xyz.com   	| 9876543678  	| Mumbai    	|
| 5     	| Rahul   	| rahul@abc.com  	| 9542456786  	| Delhi     	|

</blockquote>


<details>
<summary><b> Explanation </b></summary>

<blockquote>


      Step 1: Table is created and the values in the table is inserted.
      Step 2: To view the inserted values in the table use the `SELECT` Statement.
      Step 3: To Update the a single record use `UPDATE` Statement.
      Step 4: The Syntax for `UPDATE` Statement is 
 ```sql
                   
  UPDATE table_name
  SET column1 = value1, column2 = value2, ...
  WHERE condition;

```
</blockquote>

</details>
</details>

------

7.Predict the output of the following  for updating a Multiple record in table by using WHERE clause?
A query to update the employees EmpEmail to sample@abc.com  for all records to city name Delhi.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql
 
UPDATE Employees
Set EmpEmail = "sample@abc.com"
WHERE City = "Delhi";

```

Output:

| EmpID 	| EmpName 	| EmpEmail       	| PhoneNumber 	| City      	|
|-------	|---------	|----------------	|-------------	|-----------	|
| 1     	| Mohan   	| mohan@xyz.com  	| 9966449966  	| Delhi     	|
| 2     	| Sonia   	| sonia@abc.com  	| 9746964799  	| Mumbai    	|
| 3     	| Sanjay  	| sanjay@pqr.com 	| 9654323456  	| Bengaluru 	|
| 4     	| Avni    	| avni@xyz.com   	| 9876543678  	| Mumbai    	|
| 5     	| Rahul   	| rahul@abc.com  	| 9542456786  	| Delhi     	|

</blockquote>

<details>
<summary><b> Explanation </b></summary>

<blockquote>

To update multiple records in the table, we must use the `WHERE` clause. The `WHERE` clause determines the number of records that will be updated.

</blockquote>

</details>
</details>

------

8.Predict the output of the following  for Updating the  data by omitting `WHERE` Clause?
a query to update the employees’ emails to example@xyz.com.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

UPDATE Employees
Set EmpEmail = 'example@xyz.com’;

```
Output:
You will see the following table as output:

| EmpID 	| EmpName 	| EmpEmail       	| PhoneNumber 	| City      	|
|-------	|---------	|----------------	|-------------	|-----------	|
| 1     	| Mohan   	| mohan@xyz.com  	| 9966449966  	| Delhi     	|
| 2     	| Sonia   	| sonia@abc.com  	| 9746964799  	| Mumbai    	|
| 3     	| Sanjay  	| sanjay@pqr.com 	| 9654323456  	| Bengaluru 	|
| 4     	| Avni    	| avni@xyz.com   	| 9876543678  	| Mumbai    	|
| 5     	| Rahul   	| rahul@abc.com  	| 9542456786  	| Delhi     	|

<details>
<summary><b> Explanation </b></summary>

<blockquote>
 
When we omit the `WHERE` clause while using the `UPDATE` statement in SQL, then there is no limit set on the number of records that must be updated. So, all the records will be updated automatically.

</blockquote>

</details>
</details>

 ------

