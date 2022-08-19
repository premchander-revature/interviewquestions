1. What do you mean by Hadoop?

<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>

Hadoop was created by **Doug Cutting**, the creator of Apache Lucene, the widely used text search library. It is an **open source** as well as **distributing processing framework**, which is the key to step up into the Bigdata ecosystem. It is used to efficient store and process large datasets ranging in size from gigabytes to petabytes of data. Computer Store the large data in computer and process the data, Hadoop allows **clustering** multiple computers to analyze massive datasets in parallel more quickly.
  ![image](https://user-images.githubusercontent.com/99252558/185565924-d07c7f0a-20b9-440b-9b47-2bce55029d5a.png)
 
**Hadoop consists of four main modules:**
  
Hadoop Distributed File System (HDFS) – It allows to run on low-end hardware. HDFS provides better data throughput than traditional file systems, in addition to high fault tolerance and native support of large datasets.
  
Yet Another Resource Negotiator (YARN) – It is used to Manages and monitors cluster nodes and **resource usage**. 
  
MapReduce – MapReduce framework that helps programs do the **parallel computation** on data. The map task will take input as data and converts it into a dataset that can be computed in key value pairs. The output of the map task is consumed by reduce tasks to aggregate output and provide the desired result.
    
Hadoop Common – It Provides common Java **libraries** that can be used across all modules.

 </blockqoute> 
</details>

---


2. What do you mean by Hive?
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>

Hive is a tool which is used to work on **MapReduce** Tasks. If we think Writing a MapReduce job is **very long process and time taken**, well, with Hadoop Hive, we can used and Submit SQL queries as well as we can perform MapReduce Jobs. So, if we are comfortable with SQL Queries then Hive is a best tool for us to perform a Basic Queries which known as **HQL** (Hive Query Language. Working on HQL, we use Pig Latin as a Language.
    
Basically, Hive runs on our system, which helps to convert the SQL queries to set of jobs in Hadoop Cluster. 
    
Components of Hive:
    
1.	Driver
2.	Meta store
3.	Compiler
4.	Optimizer
5.	Executor
    
 </blockqoute> 
</details>

--- 

3. What do you mean by Spark?

<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>

Basically, **Spark** is used as a general-purpose **distributing data processing system**, which is used to use in wide range.  Spark is used as Storage as well as processing. As we know, spark has its own cluster management for computation, so it uses Hadoop storage for storing data.
    
Component of Spark:
    
1.	Spark SQL 
2.	Spark Streaming 
3.	Machine Learning 
4.	Graphx

![image](https://user-images.githubusercontent.com/70228962/185568923-3ec8184d-a9f4-4e98-b2a4-9f42d488d912.png)

    
 </blockqoute> 
</details>

--- 

4. Given that Spark is 100 times faster than Hadoop, what is the business use case for Hadoop?

<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>

 **Spark** runs a workload up to 100 times faster than **Hadoop**. 
    
Now, days in Internet has huge amount of data being generated daily, in a simple word its known as **Bigdata**. As we know data in both formats structured and Unstructured, is generated from business, organizations mainly social network. 
    
Distributed computing is used as a storing of huge data or large volume. To maintain it uses mainly Hadoop and Spark.
    
Spark is 100 times faster in memory and 10 times faster on disk. Spark is faster than Hadoop because it does the processing in **RAM **, which helps to reduce the read – write operation in system. But Spark never replace Hadoop, both are having their own way of handling data, only regarding fast processing speed we prefer spark more than Hadoop.

 </blockqoute> 
</details>

--- 



