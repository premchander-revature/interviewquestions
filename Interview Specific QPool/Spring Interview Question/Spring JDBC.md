## Spring JDBC

1. What is Spring JDBC?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
  
Spring JDBC is not separate project, but it is part of core Spring framework’s data access feature, usually referred to as Spring JDBC module. It takes care of all low level common JDBC operation and allows developer to focus only on business logic.

**Explanation**<br> Spring JDBC provides all of the Spring abstractions over the plain JDBC **DataSource** that you can use with the Spring Framework. The **JdbcTemplate** is part of this module, which allows you to execute SQL statements and extract objects from `ResultSet`s without dealing with exception handling or the nasty details of properly closing statements, connections and the like. Spring provides @Transactional annotation which can be applied on the class or on any of the methods, which allows the framework to inject transactional logic before and after the running method, mainly for starting and committing the transaction.
</blockqoute> 
</details>

---

2. What configurations does Spring JDBC & developer need to perform in application?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
  
The table shows which actions Spring takes care of and which actions are your responsibility.
  | **Steps** | **Action**                                                        | **Spring** | **Developer** |
|-----------|-------------------------------------------------------------------|------------|---------------|
|     1     |     Define   connection parameters.                               |            |     X         |
|     2     |     Open the   connection.                                        |     X      |               |
|     3     |     Specify   the SQL statement.                                  |            |     X         |
|     4     |     Declare   parameters and provide parameter values             |            |     X         |
|     5     |     Prepare   and run the statement.                              |     X      |               |
|     6     |     Set   up the loop to iterate through the results (if any).    |     X      |               |
|     7     |     Do   the work for each iteration.                             |            |     X         |
|     8     |     Process   any exception.                                      |     X      |               |
|     9     |     Handle   transactions.                                        |     X      |               |
|     10    |     Close   the connection, the statement, and the resultset.     |     X      |               |
 </blockqoute> 
</details>

---
