1. What is AWS?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- AWS stands for Amazon Web Services. It is a service which is provided by the Amazon that uses distributed IT infrastructure to provide different IT resources on demand. It provides different services such as an infrastructure as a service, platform as a service, and software as a service.

</blockquote>

</details>

---

2. What are the components of AWS?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- The following are the main components of AWS are:
  - Simple Storage Service: S3 is a service of aws that stores the files. It is object-based storage, i.e., you can store the images, word files, pdf files, etc. The size of the file that can be stored in S3 is from 0 Bytes to 5 TB. It is an unlimited storage medium, i.e., you can store the data as much you want. S3 contains a bucket which stores the files. A bucket is like a folder that stores the files. It is a universal namespace, i.e., name must be unique globally. Each bucket must have a unique name to generate the unique DNS address.
    o Elastic Compute Cloud: Elastic Compute Cloud is a web service that provides resizable compute capacity in the cloud. You can scale the compute capacity up and down as per the computing requirement changes. It changes the economics of computing by allowing you to pay only for the resources that you actually use.
    o Elastic Block Store: It provides a persistent block storage volume for use with EC2 instances in aws cloud. EBS volume is automatically replicated within its availability zone to prevent the component failure. It offers high durability, availability, and low-latency performance required to run your workloads.
    o CloudWatch: It is a service which is used to monitor all the AWS resources and applications that you run in real time. It collects and tracks the metrics that measure your resources and applications. If you want to know about the CloudWatch in detail, then click on the below link: Click here
    o Identity Access Management: It is a service of aws used to manage users and their level of access to the aws management console. It is used to set users, permissions, and roles. It allows you to grant permission to the different parts of the aws platform. If you want to know about the IAM, then click the below link: Click here
    o Simple Email Service: Amazon Simple Email Service is a cloud-based email sending service that helps digital marketers and application developers to send marketing, notification, and transactional emails. This service is very reliable and cost-effective for the businesses of all the sizes that want to keep in touch with the customers.
    o Route53: It is a highly available and scalable DNS (Domain Name Service) service. It provides a reliable and cost-effective way for the developers and businesses to route end users to internet applications by translating domain names into numeric IP addresses.

</blockquote>

</details>

---

3. What are Key-pairs?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- An Amazon EC2 uses public key cryptography which is used to encrypt and decrypt the login information. In public key cryptography, the public key is used to encrypt the information while at the receiver's side, a private key is used to decrypt the information. The combination of a public key and the private key is known as key-pairs. Key-pairs allows you to access the instances securely.

</blockquote>

</details>

---

4. What is S3?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- S3 is a storage service in aws that allows you to store the vast amount of data

</blockquote>

</details>

---

5. How many buckets can be created in S3?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- By default, you can create up to 100 buckets

</blockquote>

</details>

---

6. What is Cross Region Replication?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Cross Region Replication is a service available in aws that enables to replicate the data from one bucket to another bucket which could be in a same or different region. It provides asynchronous copying of objects, i.e., objects are not copied immediately.

</blockquote>

</details>

---

7. What are Regions and Availability Zones in aws?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Regions: A region is a geographical area which consists of 2 or more availability zones. A region is a collection of data centers which are completely isolated from other regions.

- Availability zones: An Availability zone is a data center that can be somewhere in the country or city. Data center can have multiple servers, switches, firewalls, load balancing. The things through which you can interact with the cloud reside inside the Data center.

</blockquote>

</details>

---

8. What is the minimum and maximum size that you can store in S3?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- The minimum size of an object that you can store in S3 is 0 bytes and the maximum size of an object that you can store in S3 is 5 TB.

</blockquote>

</details>

---

9. What are EBS Volumes?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Elastic Block Store is a service that provides a persistent block storage volume for use with EC2 instances in aws cloud. EBS volume is automatically replicated within its availability zone to prevent from the component failure. It offers high durability, availability, and low-latency performance required to run your workloads.

</blockquote>

</details>

---

10. What is Auto Scaling?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Auto Scaling is a feature in aws that automatically scales the capacity to maintain steady and predictable performance. While using auto scaling, you can scale multiple resources across multiple services in minutes. If you are already using Amazon EC2 Auto- scaling, then you can combine Amazon EC2 Auto-Scaling with the Auto-Scaling to scale additional resources for other AWS services.

  Benefits of Auto Scaling
  o Setup Scaling Quickly:
  It sets the target utilization levels of multiple resources in a single interface. You can see the average utilization level of multiple resources in the same console, i.e., you do not have to move to the different console.
  o Make Smart Scaling Decisions:
  It makes the scaling plans that automate how different resources respond to the changes. It optimizes the availability and cost. It automatically creates the scaling policies and sets the targets based on your preference. It also monitors your application and automatically adds or removes the capacity based on the requirements.
  o Automatically maintain performance:
  Auto Scaling automatically optimize the application performance and availability even when the workloads are unpredictable. It continuously monitors your application to maintain the desired performance level. When demand rises, then Auto Scaling automatically scales the resources.

</blockquote>

</details>

---

11. What is AMI?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- AMI stands for Amazon Machine Image. It is a virtual image used to create a virtual machine within an EC2 instance.

</blockquote>

</details>

---

12. Can a AMI be shared?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Yes, an AMI can be shared.

</blockquote>

</details>

---

13. How can you secure the access to your S3 bucket?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- S3 bucket can be secured in two ways:

o ACL (Access Control List):
ACL is used to manage the access of resources to buckets and objects. An object of each bucket is associated with ACL. It defines which AWS accounts have granted access and the type of access. When a user sends the request for a resource, then its corresponding ACL will be checked to verify whether the user has granted access to the resource or not.

    When you create a bucket, then Amazon S3 creates a default ACL which provides a full control over the AWS resources.

o Bucket Policies
Bucket policies are only applied to S3 bucket. Bucket policies define what actions are allowed or denied. Bucket policies are attached to the bucket not to an S3 object but the permissions define in the bucket policy are applied to all the objects in S3 bucket.

    The following are the main elements of Bucket policy:

    o	Sid: A Sid determines what the policy will do. For example, if an action that needs to be performed is adding a new user to an Access Control List (ACL), then the Sid would be AddCannedAcl. If the policy is defined to evaluate IP addresses, then the Sid would be IPAllow.

    o	Effect: An effect defines an action after applying the policy. The action could be either to allow an action or to deny an action.

    o	Principal: A Principal is a string that determines to whom the policy is applied. If we set the principal string as '*', then the policy is applied to everyone, but it is also possible that you can specify individual AWS account.

    o	Action: An Action is what happens when the policy is applied. For example, s3:Getobject is an action that allows to read object data.

    o	Resource: The Resource is a S3 bucket to which the statement is applied. You cannot enter a simply bucket name, you need to specify the bucket name in a specific format. For example, the bucket name is javatpoint-bucket, then the resource would be written as "arn:aws:s3""javatpoint-bucket/*".

</blockquote>

</details>

---

14. What are policies and what are the different types of policies?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Policy is an object which is associated with a resource that defines the permissions. AWS evaluate these policies when user makes a request. Permissions in the policy determine whether to allow or to deny an action. Policies are stored in the form of a JSON documents.

AWS supports six types of policies:
o Identity-based policies
o Resource-based policies
o Permissions boundaries
o Organizations SCPs
o Access Control Lists
o Session policies
![AWS policies](<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAOcAAAFzCAMAAADyqu7zAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAITUExURf///+G3tdOUksVxbsp6d7hUUOrMy9SMieCfney3tPjOzLpYVNignp+EgwAAAOW+vEU5OX5paNKurC4mJu/GxGRTUr6enKyPjdXV1bSuuJWVlX9/f4o/PHJeXpZ8e7m5uVZWVg4ODlwqKOzs7D8/PxsbG15eXnp6eyIiIujo6E5NTrWWlfv7/AcHB+Pj48bGxldQRqCgoJGJlG5ubn5+fuvPzr7Ys6PHj4y5coKzZs/jybDQo9Xo1MzgwZ3FitTlybTEsycrJztBO8XWxGx2bImViKOyo5Ogks3fzFZeVnaBdoCLf5yqnKOjo+/v7628rPLy8mhnaHNzc7PE25Ks0XiXxGyOv8nW6anA4brO6s/f9tro/MPR5LbH33iYxW92gIyVorjE1SgrLz1BRqeywVheZtLf85agrnyEkGRqdEtQV46p0cq507KYvp5+rZZzptnN38CqyuHV59XH26+Uu9DF1T87QFtWXa2jsb60wyonK3NsdpuTn4eAiq2Ruv78+OraqeLKgdq8Y9a2VvHlwte4Wu3XmPPfqPvswP/yzO/iu8S6nEdEOezgvGdiUvbpxNjNrNDFpaSbg+Dg4IJ7aC8sJsSnTrCnjXVsXo6EcZqNe+fKfOO2RdqjFdebAPDZoO3FcvPRkfvfuP/mzOOzQOvNgNjCrIJ1aLCfjfbdxGddUkdAOezUvKSUg8SwnDY2NgAAAHWtVIAAAACxdFJOU///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////ANf0XGQAAAAJcEhZcwAADsMAAA7DAcdvqGQAAB9WSURBVHhe7V2PU1RHtsZoUNmlH8iOlqm3hLwqioGXfWtRiVsi+pRgdqRSGitvjT8eDwMDasRyAMuQWGzwiZYUwiK+RLGSlBEjtVWW8y++75w+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">)
o Identity-based policies: Identity-based policies are the permissions stored in the form of JSON format. This policy can be attached to an identity user, group of users or role. It determines the actions that the users can perform, on which resources, and under what conditions.

Identity-based policies are further classified into two categories:

o Managed Policies: Managed Policies are the identity-based policies which can be attached to multiple users, groups or roles. There are two types of managed policies:

o AWS Managed Policies
AWS Managed Policies are the policies created and managed by AWS. If you are using the policies first time, then we recommend you to use AWS Managed Policies.

o Custom Managed Policies
Custom Managed Policies are the identity-based policies created by user. It provides more precise control over the policies than AWS Managed Policies.

o Inline Policies
Inline Policies are the policies created and managed by user. These policies are encapsulated directly into a single user, group or a role.

o Resource-Based Policies
Resource-based policies are the policies which are attached to the resource such as S3 bucket. Resource-based policies define the actions that can be performed on the resource and under what condition, these policies can be applied.

o Permissions boundaries
Permissions boundaries are the maximum permissions that identity-based policy can grant to the entity.

o Service Control Policies (SCPs)
Service Control Policies are the policies defined in a JSON format that specify the maximum permissions for an organization. If you enable all the features in an Organization, then you can apply Service Control Policies to any or all of your AWS accounts. SCP can limit the permission on entities in member accounts as well as AWS root user account.

o Access Control Lists (ACLs)
ACL defines the control that which principals in another AWS account can access the resource. ACLs cannot be used to control the access of a principal in a different AWS account. It is the only policy type which does not have the JSON policy document format.

</blockquote>

</details>

---

15. What are different types of instances?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Following are the different types of instances:

o General Purpose Instance type
General purpose instances are the instances mainly used by the companies. There are two types of General Purpose instances: Fixed performance (eg. M3 and M4) and Burstable performance (eg. T2). Some of the sectors use this instance such as Development environments, build servers, code repositories, low traffic websites and web applications, micro-services, etc.

Following are the General Purpose Instances:

o T2 instances: T2 instances are the instances that receive CPU credits when they are sitting idle and they use the CPU credits when they are active. These instances do not use the CPU very consistently, but it has the ability to burst to a higher level when required by the workload.

o M4 instances: M4 instances are the latest version of General purpose instances. These instances are the best choice for managing memory and network resources. They are mainly used for the applications where demand for the micro-servers is high.

o M3 instances: M3 instance is a prior version of M4. M4 instance is mainly used for data processing tasks which require additional memory, caching fleets, running backend servers for SAP and other enterprise applications.

o Compute Optimized Instance type
Compute Optimized Instance type consists of two instance types: C4 and C3.

o C3 instance: C3 instances are mainly used for those applications which require very high CPU usage. These instances are mainly recommended for those applications that require high computing power as these instances offer high performing processors.

o C4 instance: C4 instance is the next version of C3 instance. C4 instance is mainly used for those applications that require high computing power. It consists of Intel E5-2666 v3 processor and use Hardware virtualization. According to the AWS specifications, C4 instances can run at a speed of 2.9 GHz, and can reach to a clock speed of 3.5 GHz.

o GPU Instances
GPU instances consist of G2 instances which are mainly used for gaming applications that require heavy graphics and 3D application data streaming. It consists of a high-performance NVIDIA GPU which is suitable for audio, video, 3D imaging, and graphics streaming kinds of applications. To run the GPU instances, NVIDIA drivers must be installed.

o Memory Optimized Instances
Memory Optimized Instances consists of R3 instances which are designed for memory- intensive applications. R3 instance consists of latest Intel Xeon lvy Bridge processor. R3 instance can sustain a memory bandwidth of 63000 MB/sec. R3 instance offers a high- performance databases, In memory analytics, and distributed memory caches.

o Storage Optimized Instances
Storage Optimized Instances consist of two types of instances: I2 and D2 instances.

o I2 instance: It provides heavy SSD which is required for the sequential read, and write access to a large data sets. It also provides random I/O operations to your applications. It is best suited for the applications such as high-frequency online transaction processing systems, relational databases, NoSQL databases, Cache for in-memory databases, Data warehousing applications and Low latency Ad- Tech serving applications.

o D2 instance: D2 instance is a dense storage instance which consists of a high-frequency Intel Xeon E5-2676v3 processors, HDD storage, High disk throughput.

</blockquote>

</details>

---

16. What is the default storage class in S3?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- The default storage class is Standard Frequently Accessed.

</blockquote>

</details>

---

17. Difference between Stopping and Terminating the instances?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Stopping: You can stop an EC2 instance and stopping an instance means shutting down the instance. Its corresponding EBS volume is still attached to an EC2 instance, so you can restart the instance as well.

- Terminating: You can also terminate the EC2 instance and terminating an instance means you are removing the instance from your AWS account. When you terminate an instance, then its corresponding EBS is also removed. Due to this reason, you cannot restart the EC2 instance.

</blockquote>

</details>

---

18. How many Elastic IPs can you create?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- 5 elastic IP addresses that you can create per AWS account per region.

</blockquote>

</details>

---

19. What is a Load Balancer?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Load Balancer is a virtual machine that balances your web application load that could be Http or Https traffic that you are getting in. It balances a load of multiple servers so that no web server gets overwhelmed.

</blockquote>

</details>

---

20. What is VPC?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- VPC stands for Virtual Private Cloud. It is an isolated area of the AWS cloud where you can launch AWS resources in a virtual network that you define. It provides a complete control on your virtual networking environment such as selection of an IP address, creation of subnets, configuration of route tables and network gateways.

</blockquote>

</details>

---

21. What is VPC peering connection?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- A VPC peering connection is a networking connection that allows you to connect one VPC with another VPC through a direct network route using private IP addresses.
- By using VPC peering connection, instances in different VPC can communicate with each other as if they were in the same network.
- You can peer VPCs in the same account as well as with the different AWS account

</blockquote>

</details>

---

22. How can you control the security to your VPC?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- You can control the security to your VPC in two ways:

  o Security Groups
  It acts as a virtual firewall for associated EC2 instances that control both inbound and outbound traffic at the instance level. To know more about Security Groups.

  o Network access control lists (NACL)
  It acts as a firewall for associated subnets that control both inbound and outbound traffic at the subnet level. To know more about NACL

</blockquote>

</details>

---

23. What are the different database types in RDS?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Following are the different database types in RDS:
  o Amazon Aurora
  It is a database engine developed in RDS. Aurora database can run only on AWS infrastructure not like MySQL database which can be installed on any local device. It is a MySQL compatible relational database engine that combines the speed and availability of traditional databases with the open source database.

  o Postgre SQL
  PostgreSQL is an open source relational database for many developers and startups.
  It is easy to set up, operate, and can also scale PostgreSQL deployments in the cloud.
  You can also scale PostgreSQL deployments in minutes with cost-efficient.
  PostgreSQL database manages time-consuming administrative tasks such as PostgreSQL software installation, storage management, and backups for disaster recovery.

  o MySQL
  It is an open source relational database.
  It is easy to set up, operate, and can also scale MySQL deployments in the cloud.
  By using Amazon RDS, you can deploy scalable MySQL servers in minutes with cost-efficient.

  o MariaDB
  It is an open source relational database created by the developers of MySQL.
  It is easy to set up, operate, and can also scale MariaDB server deployments in the cloud.
  By using Amazon RDS, you can deploy scalable MariaDB servers in minutes with cost-efficient.
  It frees you from managing administrative tasks such as backups, software patching, monitoring, scaling and replication.

  o Oracle
  It is a relational database developed by Oracle.
  It is easy to set up, operate, and can also scale Oracle database deployments in the cloud.
  You can deploy multiple editions of Oracle in minutes with cost-efficient.
  It frees you from managing administrative tasks such as backups, software patching, monitoring, scaling and replication.
  You can run Oracle under two different licensing models: "License Included" and "Bring Your Own License (BYOL)". In License Included service model, you do need have to purchase the Oracle license separately as it is already licensed by AWS. In this model, pricing starts at $0.04 per hour. If you already have purchased the Oracle license, then you can use the BYOL model to run Oracle databases in Amazon RDS with pricing starts at $0.025 per hour.

  o SQL Server

  SQL Server is a relational database developed by Microsoft.
  It is easy to set up, operate, and can also scale SQL Server deployments in the cloud.
  You can deploy multiple editions of SQL Server in minutes with cost-efficient.
  It frees you from managing administrative tasks such as backups, software patching, monitoring, scaling and replication.

</blockquote>

</details>

---

24. What is Redshift?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Redshift is a fast, powerful, scalable and fully managed data warehouse service in the cloud.
- It provides ten times faster performance than other data warehouse by using machine learning, massively parallel query execution, and columnar storage on high-performance disk.
- You can run petabytes of data in Redshift datawarehouse and exabytes of data in your data lake built on Amazon S3.

</blockquote>

</details>

---

25. What are the different types of routing policies in route53?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- Following are the different types of routing policies in route53:

- Simple Routing Policy

  Simple Routing Policy is a simple round-robin policy which is applied to a single resource doing the function for the domain, For example, web server is sending the content to a website where web server is a single resource.
  It responds to DNS queries based on the values present in the resource.

- Weighted Routing Policy

  Weighted Routing Policy allows you to route the traffic to different resources in specified proportions. For example, 75% in one server, and 25% in another server.
  Weights can be assigned in the range from 0 to 255.

  Weight Routing policy is applied when there are multiple resources accessing the same function. For example, web servers accessing the same website. Each web server will be given a unique weight number.

  Weighted Routing Policy associates the multiple resources to a single DNS name.

- Latency-based Routing Policy
  Latent-based Routing Policy allows Route53 to respond to the DNS query at which data center gives the lowest latency.
  Latency-based Routing policy is used when there are multiple resources accessing the same domain. Route53 will identify the resource that provides the fastest response with lowest latency.

- Failover Routing Policy
- Geolocation Routing Policy

</blockquote>

</details>

---

26. What is the maximum size of messages in SQS?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- The maximum size of message in SQS IS 256 KB.

</blockquote>

</details>

---

27. Differences between Security group and Network access control list?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

| **Security Group**                                                                                                                                                                                                                   | **NACL (Network Access Control List)**                                                                                                                                                                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| It supports only allow rules, and by default, all the rules are denied. You cannot deny the rule for establishing a connection.                                                                                                      | It supports both allow and deny rules, and by default, all the rules are denied. You need to add the rule which you can either allow or deny it.                                                                                                                          |
| It is a stateful means that any changes made in the inbound rule will be automatically reflected in the outbound rule. For example, If you are allowing an incoming port 80, then you also have to add the outbound rule explicitly. | It is a stateless means that any changes made in the inbound rule will not reflect the outbound rule, i.e., you need to add the outbound rule separately. For example, if you add an inbound rule port number 80, then you also have to explicitly add the outbound rule. |
| It is associated with an EC2 instance.                                                                                                                                                                                               | It is associated with a subnet.                                                                                                                                                                                                                                           |
| All the rules are evaluated before deciding whether to allow the traffic.                                                                                                                                                            | Rules are evaluated in order, starting from the lowest number.                                                                                                                                                                                                            |
| Security Group is applied to an instance only when you specify a security group while launching an instance.                                                                                                                         | NACL has applied automatically to all the instances which are associated with an instance.                                                                                                                                                                                |
| It is the first layer of defense.                                                                                                                                                                                                    | It is the second layer of defense.                                                                                                                                                                                                                                        |

</blockquote>

</details>

---

28. What are the two types of access that you can provide when you are creating users?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- There are two types of access:

  - Console Access
    If the user wants to use the Console Access, a user needs to create a password to login in an AWS account.

  - Programmatic access
    If you use the Programmatic access, an IAM user need to make an API calls. An API call can be made by using the AWS CLI. To use the AWS CLI, you need to create an access key ID and secret access key.

</blockquote>

</details>

---

29. What is subnet?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

- When large section of IP address is divided into smaller units is known as subnet.

- A Virtual Private Cloud (VPC) is a virtual network provided to your AWS account. When you create a virtual cloud, you need to specify the IPv4 addresses which is in the form of CIDR block. After creating a VPC, you need to create the subnets in each availability zone. Each subnet has a unique ID. When launching instances in each availability zone, it will protect your applications from the failure of a single location.

</blockquote>

</details>

---

30. Differences between Amazon S3 and EC2?

![Easy](<https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg>)

<details>
<summary> <b>Explanation</b> </summary>

<blockquote>

S3

- It is a storage service where it can store any amount of data.
- It consists of a REST interface and uses secure HMAC-SHA1 authentication keys.

EC2

- It is a web service used for hosting an application.
- It is a virtual machine which can run either Linux or Windows and can also run the applications such as PHP, Python, Apache or other databases.

</blockquote>

</details>

---
