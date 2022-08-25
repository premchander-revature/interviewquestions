1.Write a syntax for Inserting a Specific column in a table.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

INSERT INTO Student(ROLL_NO,NAME,Age) SELECT ROLL_NO, NAME, Age FROM  Lateral_Student;

```

| Roll_No 	| Name    	| Address   	| Ph_No      	| Age 	|
|-----------|-----------|-----------------|-----------------|-----------|
| 1       	| Ram     	| Delhi     	| 6789043256 	| 18  	|
| 2       	| Ramesh  	| Chennai   	| 8765432165 	| 23  	|
| 3       	| Suresh  	| Raipur    	| 9876543217 	| 20  	|
| 4       	| Sneha   	| Pune      	| 9087453261 	| 17  	|
| 5       	| Pooja   	| Kerala    	| 6754839201 	| 34  	|
| 6       	| Revathi 	| Karnataka 	| 8976346229 	| 65  	|
| 7       	| Krishna 	| Bangalore 	| 7854779326 	| 48  	|
| 8       	| Divya   	| Hyderabad 	| 8734652705 	| 59  	|
| 9       	| Keethi  	| Andhra    	| 9846883463 	| 63  	|

<details>
<summary><b> Explanation </b></summary>

<blockquote>

This query will insert the data in the columns ROLL_NO, NAME and Age of the table Student in the 
table Student and the remaining columns in the Student table will be filled by null which is the 
default value of the remaining columns. 

</blockquote>

</details>
</details>
------

2.How will you Delete the multiple records from the following given table below: 

| Roll_No 	| Name    	| Address   	| Ph_No      	| Age 	|
|-----------|-----------|-----------------|-----------------|-----------|
| 1       	| Ram     	| Delhi     	| 6789043256 	| 18  	|
| 2       	| Ramesh  	| Chennai   	| 8765432165 	| 23  	|
| 3       	| Suresh  	| Raipur    	| 9876543217 	| 20  	|
| 4       	| Sneha   	| Pune      	| 9087453261 	| 17  	|
| 5       	| Pooja   	| Kerala    	| 6754839201 	| 34  	|
| 6       	| Revathi 	| Karnataka 	| 8976346229 	| 65  	|
| 7       	| Krishna 	| Bangalore 	| 7854779326 	| 48  	|
| 8       	| Divya   	| Hyderabad 	| 8734652705 	| 59  	|
| 9       	| Keethi  	| Andhra    	| 9846883463 	| 63  	|

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

DELETE FROM Student WHERE Age > 20;

```

Delete the rows from the table Student where Age is 20.

| Roll_No 	| Name    	| Address   	| Ph_No      	| Age 	|
|-----------|-----------|-----------------|-----------------|-----------|
| 1       	| Ram     	| Delhi     	| 6789043256 	| 18  	|
| 3       	| Suresh  	| Raipur    	| 9876543217 	| 20  	|
| 4       	| Sneha   	| Pune      	| 9087453261 	| 17  	|

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Explanation </b></summary>

<blockquote>

The above query will delete where the age is above 20 from the given table and the syntax for Deleting the multiple records is,

     `DELETE` FROM Table_Name `WHERE` Condition;
</blockquote>

</details>
</details>
------

3.How will you Delete a single record in the given table.

| Roll_No 	| Name    	| Address   	| Ph_No      	| Age 	|
|---------	|---------	|-----------	|------------	|-----	|
| 1       	| Ram     	| Delhi     	| 6789043256 	| 18  	|
| 2       	| Divya   	| Chennai   	| 8765432165 	| 23  	|
| 3       	| Suresh  	| Raipur    	| 9876543217 	| 20  	|
| 4       	| Sneha   	| Pune      	| 9087453261 	| 17  	|
| 5       	| Divya   	| Kerala    	| 6754839201 	| 34  	|
| 6       	| Revathi 	| Karnataka 	| 8976346229 	| 65  	|
| 7       	| Krishna 	| Bangalore 	| 7854779326 	| 48  	|
| 8       	| Divya   	| Hyderabad 	| 8734652705 	| 59  	|
| 9       	| Keethi  	| Andhra    	| 9846883463 	| 63  	|

Delete the rows where NAME = "Divya".

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

DELETE FROM Student WHERE NAME = "Divya";

```

|    Roll_No  |     Name     |    Address    |        Ph_No       |   Age   |
|-------------|--------------|---------------|--------------------|---------|
|      1	    |     Ram      |	   Delhi	   |      6789043256    |  18     |
|      3	    |    Suresh    |    Raipur	   |      9876543217    |  20     |
|      4	    |    Sneha     |	   Pune      |      9087453261    |  17     |
|      6	    |    Revathi   |   Karnataka   |      8976346229    |  65     |
|      7	    |    Krishna   |   Bangalore   |      7854779326    |	 48     |
|      9	    |    Keethi    |	  Andhra	   |      9846883463    |	 63     |

<details>
<summary><b> Explanation </b></summary>

<blockquote>

The above query will delete only the particular row where name="Divya" by using delete command.
`DELETE` FROM Table_Name `WHERE` Condition;
</blockquote>

</details>
</details>
------

4.How will you Update multiple columns in the given below table

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

Update the columns NAME to "PRATIK" and ADDRESS to "CHENNAI" where ROLL_NO is 1.

```sql

UPDATE Student SET NAME = "PRATIK", ADDRESS = "CHENNAI" WHERE ROLL_NO = 1;

```

| Roll_No 	| Name   	| Address    	| Ph_No      	| Age 	|
|---------	|--------	|------------	|------------	|-----	|
| 1       	| PRATIK 	| CHENNAI    	| 6875064321 	| 18  	|
| 2       	| RAMESH 	| GURGAON    	| 9944006573 	| 18  	|
| 3       	| PRATIK 	| ROHTAK     	| 7904567890 	| 20  	|
| 4       	| SURESH 	| Bangalore  	| 8898655777 	| 18  	|
| 5       	| PRATIK 	| Rajasthan  	| 8746483738 	| 20  	|
| 6       	| RAMESH 	| DELHI      	| 9876453722 	| 18  	|

<details>
<summary><b> Explanation </b></summary>

<blockquote>

The above query will updated two columns in the first row and the table Student.

For updating multiple columns we have used comma(,) to separate the names and values of two columns. 

</blockquote>

</details>
</details>
------

5.How can you update the records of a table from another table in sql?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

CREATE TABLE demo_table1(
ID int,
NAME VARCHAR(20),
AGE INT,
CITY VARCHAR(20) );

```

```sql
      INSERT INTO demo_table1 VALUES(1,"Rocky",23,"Chennai");
                                    (2,"Rahul",23,"Delhi"),
                                    (3,"Divya",24,"Punjab"),
                                    (4,"Ranvir",23,"Punjab"),
                                    (5,"Samiksha",23,"Banglore"),
                                    (6,"Ashtha",24,"Banglore"),
                                    (7,"Tannu",30,"Patna"),
                                    (8,"Girish",30,"Patna"),
                                    (9,"Ram", 20 , "Patna"),
                                    (10,"Raj", 12, "Delhi");

```

| ID 	| NAME     	| AGE 	| CITY     	|
|----	|----------	|-----	|----------	|
| 1  	| Rocky    	| 23  	| Chennai  	|
| 2  	| Rahul    	| 23  	| Delhi    	|
| 3  	| Divya    	| 24  	| Punjab   	|
| 4  	| Ranvir   	| 23  	| Punjab   	|
| 5  	| Samiksha 	| 23  	| Banglore 	|
| 6  	| Ashtha   	| 24  	| Banglore 	|
| 7  	| Tannu    	| 30  	| Patna    	|
| 8  	| Girish   	| 30  	| Patna    	|
| 9  	| Ram      	| 20  	| Patna    	|
| 10 	| Raj      	| 12  	| Delhi    	|

```sql

CREATE TABLE demo_table2(
ID int,
NAME VARCHAR(20),
AGE int);

```

```sql

INSERT INTO demo_table2 VALUES(3,'Fanny',25 );
INSERT INTO demo_table2 VALUES(7,'Prem', 30);
INSERT INTO demo_table2 VALUES(1,'Preeti',21);
INSERT INTO demo_table2 VALUES(4,'Samita',32);

```

|  ID  |  NAME  |  ID  |
|------|--------|------|
|  3   | Fanny  |	 25  |
|  7   | Prem   |	 30  |
|  1   | Preeti |	 21  |
|  4   | Samita |	 32  |

```sql

UPDATE demo_table1 SET demo_table1.NAME=demo_table2.NAME, demo_table1.AGE=demo_table2.AGE FROM demo_table1, demo_table2  WHERE demo_table1.ID=demo_table2.ID;

```

<details>
<summary><b> Explanation </b></summary>

<blockquote>

By Using the SQL `UPDATE` statement, we may update the table. The `SET` command always comes after the update statement.

To define which columns and values in a table need to be modified, we could use the `SET` command.

UPDATE syntax:
```sql

UPDATE table_name
SET column_name = value
WHERE condition;

```
</blockquote>

</details>
</details>
------

6.How can you update the gender column of the table to  MN' IF 1,'F' OF 2,AND 'U' IF NULL?

```sql

      CREATE TABLE EMP_DATA(
       EMPNAME VARCHAR(25),
       GENDER VARCHAR(6),
       DEPT VARCHAR(20),
       CONTACTNO BIGINT NOT NULL,
       CITY VARCHAR(15));

```

```sql

INSERT INTO EMP_DATA VALUES ("Vishal", "Male", "Sales", 9193458625, "Gaziabad"),
                            ("Divya", "Female", "Manager",7352158944, "Barielly"),
                            ("Rekha", "Female", "IT", 7830246946, "Kolakata"),
                            ("Rahul", "Male", "Marketing", 9635688441, "Meerut"),
                            ("Sanjay", "Male", "Sales", 9149335694, "Moradabad"),
                            ("Rohan", "Male", "Manager", 7352158944, "Bengaluru"),
                            ("Rajshree", "Female", "Sales", 9193458625, "Vododara"),
                            ("Aman", "Male", "IT", 78359941265, "Rampur"),
                            ("Rakesh", "Male", "Marketing", 9645956441, "Bokaro"),
                            ("Mohini", "Female", "Sales", 9147844694, "Dehli");

```

```sql

 SELECT * FROM EMPDATA;
 
 ```
 
| EMPNAME  	| GENDER  	| DEPT        	| CONTACTNO   	| CITY      	|
|----------	|---------	|-------------	|-------------	|-----------	|
| VISHAL   	| MALE    	| SALES       	| 9193458625  	| GAZIABAD  	|
| DIVYA    	| FEMALE  	| MANAGER     	| 7352158944  	| BARIELLY  	|
| REKHA    	| FEMALE  	| IT          	| 7830246946  	| KOLKATA   	|
| RAHUL    	| MALE    	| MARKETING\| 	| 9635688441  	| MEERUT    	|
| SANJAY   	| MALE    	| SALES       	| 9149335694  	| MORADABAD 	|
| ROHAN    	| MALE    	| MANAGER     	| 7352158944  	| BENGALURU 	|
| RAJSHREE 	| FEMALE  	| SALES       	| 9193458625  	| VODODARA  	|
| AMAN     	| MALE    	| IT          	| 78359941265 	| RAMPUR    	|
| RAKESH   	| MALE    	| MARKETING   	| 9645956441  	| BOKARO    	|
| MOHINI   	| FEMALE  	| SALES       	| 9147844694  	| Dehli     	|

 ![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

Correct Answer:

| EMPNAME  	| GENDER  	| DEPT      	| CONTACTNO   	| CITY      	|
|----------	|---------	|-----------	|-------------	|-----------	|
| VISHAL   	| MALE    	| SALES     	| 9193458625  	| GAZIABAD  	|
| DIVYA    	| FEMALE  	| MANAGER   	| 7352158944  	| BARIELLY  	|
| REKHA    	| FEMALE  	| IT        	| 7830246946  	| KOLKATA   	|
| RAHUL    	| MALE    	| MARKETING 	| 9635688441  	| MEERUT    	|
| SANJAY   	| MALE    	| SALES     	| 9149335694  	| MORADABAD 	|
| ROHAN    	| MALE    	| MANAGER   	| 7352158944  	| BENGALURU 	|
| RAJSHREE 	| FEMALE  	| SALES     	| 9193458625  	| VODODARA  	|
| AMAN     	| MALE    	| IT        	| 78359941265 	| RAMPUR    	|
| RAKESH   	| MALE    	| MARKETING 	| 9645956441  	| BOKARO    	|
| MOHINI   	| FEMALE  	| SALES     	| 9147844694  	| Dehli     	|

<details>
<summary><b> Explanation </b></summary>

<blockquote>
     The Update command is used to update the data in the table and the syntax is ,
                 `UPDATE` [EMP_DATA] `SET` GENDER = "FEMALE" `WHERE` EMPNAME = "AMAN";
</blockquote>

</details>
</details>
------

7.How can you get the last inserted record ID?

```sql

create table Patient_Details(pat_Id int,
    Pat_Name varchar(20),  
    Pat_Age int);

```

```sql

insert into Patient_Details values(6455, "Shanmuganathan", 56);
insert into Patient_Details values(4533, "Sakthivel", 70);
insert into Patient_Details values(5425, "Lakshmi", 68);
insert into Patient_Details values(2367, "Mahalakshmi", 55);
insert into Patient_Details values(4875, "Gopinath", 45);

```

```sql

select*from Patient_Details;

``` 

| pat_Id 	| Pat_Name       	| Pat_Age 	|
|--------	|----------------	|---------	|
| 6455   	| Shanmuganathan 	| 56      	|
| 4533   	| Sakthivel      	| 70      	|
| 5425   	| Lakshmi        	| 68      	|
| 2367   	| Mahalakshmi    	| 55      	|
| 4875   	| Gopinath       	| 45      	|

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

select Pat_id(3);

```  
| pat_Id 	|
|--------	|
| 4875   	|                
             
If you want the entire row, then use the following query

```sql

select *from LastInsertedRow where Id=(SELECT LAST_INSERT_ID());

```

The following is the output
                  
| pat_Id 	| Pat_Name 	| Pat_Age 	|
|--------	|----------	|---------	|
| 4875   	| Gopinath 	| 45      	|

<details>
<summary><b> Explanation </b></summary>

<blockquote>                  

The syntax for inserting the query 

```sql

select Pat_id();

```

</blockquote>

</details>
</details>
------

8.Populate the table WEATHER_MONITOR adding couple of rows.

Table: WEATHER_MONITOR

| ID  	| CITY       	| STATE      	| TEMP 	| LATITUDE_N 	| LONGITUDE_W 	|
|-----	|------------	|------------	|------	|------------	|-------------	|
| 10  	| HOUSTON    	| TEXAS      	| 15.6 	| 33         	| 112         	|
| 123 	| LOS ANGELS 	| CALIFORNIA 	| 18.3 	| 45         	| 134         	|

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

INSERT INTO WEATHER_MONITOR VALUES (10, HOUSTON,TEXAS, 15.6, 33, 112 );
INSERT INTO WEATHER_MONITOR VALUES (123,LOS ANGELS, CALIFORNIA,18.3,45,134 );

```


<details>
<summary><b> Explanation </b></summary>

<blockquote>

    It is achieved by using `INSERT` command present in Data Manipulation Language.
</blockquote>

</details>
</details>
------

9.Let's take the following  table called Student, in which it consists of only 2 records of the table named Student.

| Stu_Id 	| Stu_Name 	| Stu_Marks 	| Stu_Age 	|
|--------	|----------	|-----------	|---------	|
| 101    	| Ramesh   	| 92        	| 20      	|
| 201    	| Kavitha  	| 83        	| 19      	|

Suppose, if you want to insert a new record into the student table. for this you have to write the following DML `INSERT` command:

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

INSERT INTO Student VALUES (104, "Divya", 89, 19);  

```

<details>
<summary><b> Explanation </b></summary>

<blockquote>
 
If you want to insert a record into the given table we can use the DML `INSERT` command and the Syntax for inserting a record in the given table is,

`INSERT` INTO table_name `VALUES` (value1, value2, value3, ...);

                         (OR)

`INSERT` INTO table_name (column1, column2, column3, ...) `VALUES` (value1, value2, value3, ...);

</blockquote>

</details>
</details>
------

10.How to remove duplicate rows in from a table in SQL?

If the table has some duplicate rows, the duplicate rows must be removed.

Let’s assume the following table as our dataset:

 

| ID 	| Name     	| Age 	|
|----	|----------	|-----	|
| 1  	| Divya    	| 21  	|
| 2  	| Vinoth   	| 23  	|
| 3  	| Tharun   	| 23  	|
| 4  	| Renuka   	| 22  	|
| 5  	| Pavithra 	| 25  	|
| 6  	| Ganesh   	| 26  	|
| 7  	| Sandhiya 	| 25  	|

The following SQL query removes the duplicate ids from the  table:
![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

DELETE FROM table WHERE ID IN (
SELECT 
ID, COUNT(ID) 
FROM   table
GROUP BY  ID
HAVING 
COUNT (ID) > 1);

```
<details>
<summary><b> Explanation </b></summary>

<blockquote>

If you want to remove the duplicate in  a record into the given table we can use the DML `GROUP BY` command.

</blockquote>

</details>
</details>
------

11.How to insert a data through SELECT Statement?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

create table Student(stu_id int, stu_name varchar(20),
stu_age int,
stu_mail_id text,
stu_contact_no text); 

```

```sql

insert into Student(1, "Aswitha", 21, "aswitha@gmail.com", 9876543210);
insert into Student(2, "Divya", 20, "divyawe@gmail.com",   9665273450);
insert into Student(3, "Harshini", 22, "harshini543@gmail.com", 9832167455);
insert into Student(4, "Poornima", 20, "poorniapj@gmail.com", 8734562777);
insert into Student(5, "Gayathrii", 21, "gayathri123@gmail.com", 9441234587);

```

```sql

select * from Student;

```

| stu_id 	| stu_name  	| stu_age 	| stu_mail_id           	| stu_contact_no 	|
|--------	|-----------	|---------	|-----------------------	|----------------	|
| 1      	| Aswitha   	| 21      	| aswitha@gmail.com     	| 9876543210     	|
| 2      	| Divya     	| 20      	| divyawe@gmail.com     	| 9665273450     	|
| 3      	| Harshini  	| 22      	| harshini543@gmail.com 	| 9832167455     	|
| 4      	| Poornima  	| 20      	| poorniapj@gmail.com   	| 8734562777     	|
| 5      	| Gayathrii 	| 21      	| gayathri123@gmail.com 	| 9441234587     	|

```sql
insert into studentg( stu_id, stu_name, stu_age, stu_mail_id, stu_contact_no)
SELECT stu_id, stu_name, stu_age, stu_mail_id, stu_contact_no
FROM studentg WHERE stu_id = 1;

```

```sql

select * from Studentg  WHERE stu_id = 1;

```

Output:

   |   stu_id    |     stu_name      |  stu_age  |          stu_mail_id           |    stu_contact_no   | 
   |-------------|-------------------|-----------|--------------------------------|---------------------|
   |     1       |    	Aswitha	 |    21	 |       aswitha@gmail.com        |     9876543210      |
   |     1       |    	Aswitha	 |    21	 |       aswitha@gmail.com        |	     9876543210     |
   |     1       |    	Aswitha	 |    21	 |       aswitha@gmail.com        |	     9876543210     |
   |     1       |    	Aswitha	 |    21	 |       aswitha@gmail.com        |	     9876543210     |        
<details>
<summary><b> Explanation </b></summary>

<blockquote>
 
 Data from one table is copied and inserted into another table using the INSERT INTO SELECT query. The data types in the source and target tables must coincide for the `INSERT` INTO `SELECT` query to work. Notably, the target table's current records remain unaffected and it is used by using only one table.

The Syntax for inserting a data through `SELECT` Statement.

```sql

INSERT  INTO table_name  
[(column1, column2, .... column)]  
SELECT column1, column2, .... Column N  
FROM table_name [WHERE condition]; 

```

</blockquote>

</details>
</details>
------

12.How to INSERT a Multiple Records by placing a SELECT statement within the INSERT statement, you can perform multiples inserts quickly. 

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

In this example, we have a table called Employee with the following data:
```sql

create table Employee(employee_number  int, last_name varchar(20), first_name	 varchar(20), salary int,  dept_id int);

```

```sql

insert into Employee values( 10001, "Daniel",  "Smith", 62000 , 5234);
insert into Employee values( 10002, "Divya", "Lakshmi", 57500, 5067);
insert into Employee values( 10003, "Balaji", "Dev", 71000, 2501);
insert into Employee values( 10004, "Harish", "Kumar", 42000, 3876);
insert into Employee values( 10005, "Karthiga", "Bhavani", 35000, 6589);

```

```sql

select * from Employee;

```

|   employee_number  | 	last_name	|  first_name |  salary  | 	dept_id |
|--------------------|--------------|-------------|----------|------------|
|        10001	   |    Daniel    |    Smith 	  |	 62000 |   	5234    |
|        10002	   |     Divya    |    Lakshmi  |	 57500 |    5067    |
|        10003	   |    Balaji    |    Dev      |	 71000 |	2501    |
|        10004	   |	  Harish    |    Kumar    |    42000 |	3876    |
|        10005       |   Karthiga   |    Bhavani  |    35000 |    6589    |
And a table called customers with the following data:

```sql 

create table Customers( customer_id   int, last_name  varchar(20), first_name varchar(20),  favorite_website  text);

```

```sql

insert into Customers values(4321, "Kumar", "Vinoth", "techonthenet.com");
insert into Customers values(4523, "Smith",	"Jane", "digminecraft.com");
insert into Customers values( 6537, "Hari", "Prasad", "bigactivities.com");
insert into Customers values( 2000, "John", "Daniel", "checkyourmath.com");
insert into Customers values( 3334, "Dilip", "Babu", "NULL" );
insert into Customers values( 9567, "Ashwath", "Kumaravel", "techonthenet.com" );

```

```sql

select * from Customers;

```

|    customer_id     |  last_name         |  	first_name	  |   favorite_website   |
|--------------------|--------------------|-------------------|----------------------|
|       4321         |	    Kumar         |	 Vinoth       |    techonthenet.com  |
|       4523         |	   Smith	      |     Jane          |	 digminecraft.com  |
|       6537         |	    Hari          |	Prasad	  |    bigactivities.com |
|       2000	   |      John          |     Daniel        |	 checkyourmath.com |
|       3334	   |     Dilip	      |     Babu	        |       NULL           |
|       9567	   |    Ashwath         |	Kumaravel     |	 techonthenet.com  |

Now, let's insert some of the employee information into the customers table:

```sql

INSERT INTO Customers(customer_id, last_name, first_name)
SELECT employee_number AS customer_id, last_name, first_name
FROM Employees
WHERE employee_number < 1003;

```

There will be 2 records inserted. Select the data from the customers table again:

```sql

SELECT * FROM customers;

```

These are the results that you should see:
        

|    customer_id     |   last_name   |  	first_name	  |   favorite_website   |
|--------------------|---------------|------------------|----------------------|
|       4321         |	    Kumar    |	  Vinoth      |    techonthenet.com  |
|       4523         |	   Smith	 |       Jane       |	   digminecraft.com|
|       6537         |	    Hari     |	   Prasad	  |    bigactivities.com |
|       2000	   |      John     |      Daniel      |	 checkyourmath.com |
|       3334	   |     Dilip	 |       Babu	  |       NULL           |
|       9567	   |    Ashwath    |	   Kumaravel  |	 techonthenet.com  |
|      10001	   |    Daniel     |       Smith 	  |	    NULL           |   	
|      10002	   |     Divya     |	   Lakshmi    |	    NULL           | 

In this example, the last 2 records in the customers table have been inserted using data from the employees table.

With this type of insert, you may wish to check for the number of rows being inserted. You can determine the number of rows that will be inserted by running a `COUNT`(*) on the `SELECT` statement before performing the insert. For example:
```sql

SELECT COUNT(*)
FROM Employee
WHERE employee_number < 1003;

```

| employee_number 	| last_name 	| first_name 	| salary 	| dept_id 	|
|-----------------	|-----------	|------------	|--------	|---------	|
| 10001           	| Daniel    	| Smith      	| 62000  	| 5234    	|
| 10002           	| Divya     	| Lakshmi    	| 57500  	| 5067    	|

This will return number of records that will be inserted when you execute the INSERT statement.

<details>
<summary><b> Explanation </b></summary>

<blockquote>


 With this type of `INSERT`, some databases require you to alias the column names in the `SELECT` to match the column names of the table you are inserting into. As you can see in the example above, we have aliased the first column in the `SELECT` statement to customer_id.
</blockquote>

</details>
</details>
 