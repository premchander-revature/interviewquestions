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
