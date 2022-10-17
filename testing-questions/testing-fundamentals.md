1. What is Software testing?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Software testing is the process of evaluating and verifying that a software product or application does what it is supposed to do.

</blockquote>
</details>
  
---

2. Why do we need to do testing?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Some reasons:

- Since it discovers defects/bugs before the delivery to the client, which guarantees the high quality of the software.
- It makes the software more reliable and easy to use.
- Thoroughly tested software ensures reliable and high-performance software operation.

</blockquote>
</details>
  
---

3. What is manual software testing, and how does it differ from automated software testing?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Manual software testing is a process where human testers manually run test cases, then generate the resulting test reports. With automation software testing, these functions are executed by automation tools such as test scripts and code. The tester takes the end user’s role to determine how well the app works.

</blockquote>
</details>
  
---


4. What is meant by STLC?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

- STLC stands Software Testing Life Cyle. 
- STLC defines a series of activities performed during testing to ensure the quality of the software.
  
<img src = "https://user-images.githubusercontent.com/70228962/195261473-9140741d-0315-405c-ac06-def823ea023d.png" height="300"/>
 
**6 Phases:**
  
1. **Requirement Analysis** - During this phase, feature requirements collected in the SDLC process are evaluated to identify testable aspects. If necessary, testing teams may need to consult with stakeholders to clarify requirements. These requirements can either be functional or non-functional, defining what a feature can do or it’s characteristics respectively.
2. **Test Planning** - This phase includes implementing and defining a test strategy in the testing plan and estimating the efforts and costs of the testing team. 
3. **Test Case Development** - During this phase, testers create test cases. Each test case defines test inputs for data, procedures, execution conditions, and anticipated results.
4. **Environment Setup** - 
5. **Test Execution** - 
6. **Test Closure** - 

</blockquote>
</details>
  
---

5. List the types of testing


![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
  
Software testing is generally classified into two main broad categories: functional testing and non-functional testing.

![image](https://user-images.githubusercontent.com/70228962/195307040-d274cee8-d794-49c9-9081-e552c24d3096.png)

<img src = "https://user-images.githubusercontent.com/70228962/195267678-4f17c0c7-71b7-4210-8ae9-7d1e4cc15af9.png" height = "300"/>

</blockquote>
</details>
  
---

What is meant by entry criteria and exit criteria?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
  
Entry Criteria: Entry Criteria are a set of conditions that need to be satisfied in order to begin the test.
Exit Criteria: Exit Criteria are a set of conditions that need to be satisfied in order to end the test.

What is the purpose of the test closure phase?
  
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
  
Test closure activities have several purposes, such as to:

Make sure testing is completed.
Gather and submit test artifacts.
Hold retrospective meetings to review previous information and improve.

What is the difference between SDLC and STLC?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote> 
  
Software Development Life Cycle (SDLC) is a process of software development, presented as a set of sequential phases such as:

Planning
Analysis and Design
Implementation (Coding)
Testing
Deployment and Maintenance (in some sources called ‘Evolution,’ to emphasize the importance of Retrospective analysis and Lessons Learned practices which become a background for another software development cycle)
So it can be said that the Software Testing Life Cycle is a part of the Software Development Life Cycle, and represents testing activities held within it. A rule of thumb is to have a testing activity for every development activity, and to start it as early as possible. For instance, test design for each test level should start in parallel with the corresponding development activity.


What is white box testing with example?

White box testing techniques analyze the internal structures the used data structures, internal design, code structure and the working of the software rather than just the functionality as in black box testing. It is also called glass box testing or clear box testing or structural testing.

What is black box testing with example?
Image result for white box testing and black box testing
Black box testing can test specific functions or features of the software under test. For example, checking that it is possible to log in using correct user credentials, and not possible to log in using wrong credentials.


Which is “better” – white or black box testing?
Neither – they are both necessary and complementary. Early white box testing assures code functionality and makes later, higher level testing less time intensive. Thorough black box testing enhances end user experience. Systematic testing procedures, incorporating a variety of strategies and perspectives, result in a solid final product and a successful release.

What are the differences between white box and black box testing?
White box testing usually begins early in the development cycle. It is conducted at lower levels, and includes unit and integration testing. Black box testing is mainly higher level, as in system and acceptance testing, so implementation comes later in the development cycle.

 What is Verification and Validation in Software Testing?
Verification: It is a static analysis technique. Here, testing is done without executing the code. Examples include – Reviews, Inspection, and walkthrough.

Validation: It is a dynamic analysis technique where testing is done by executing the code. Examples include functional and non-functional testing techniques.

What is the difference between a feature and a bug?
A feature is a functionality intended to be useful to the user. A bug is a behavior, usually the result of an error or sloppy programming, that gets in the way of the features.

Difference between Bug and Defect
+-------------------------------------------------------+---------------------------------------------------------------------------------------------------------+
| BUG                                                   | DEFECT                                                                                                  |
+-------------------------------------------------------+---------------------------------------------------------------------------------------------------------+
| A bug is a deviation from the customer’s requirement. | The functionality of an application not working as per the customer’s requirement is known as a defect. |
+-------------------------------------------------------+---------------------------------------------------------------------------------------------------------+
| The bug is found by the testing team.                 | The defect is found by the development team.                                                            |
+-------------------------------------------------------+---------------------------------------------------------------------------------------------------------+
| Reason Behind Bug:                                    | Reason Behind Defect:                                                                                   |
|                                                       |                                                                                                         |
| Missing Coding                                        | Giving wrong input may lead to a defect.                                                                |
| Wrong Coding                                          | Any error in code may lead to a defect.                                                                 |
| Extra Coding                                          |                                                                                                         |
+-------------------------------------------------------+---------------------------------------------------------------------------------------------------------+


What is error, bug, defect anf failure?

A mistake made by a programmer during coding is called an error, an error found during the unit testing in the development phase is called a defect, an error found during the testing phase is called a bug and when an error is found at an end user’s end is called as the failure.

What is Defect/Bug Life Cycle in Software Testing?

The Defect Life Cycle is also known as Bug Life Cycle. It is a process in which bug goes through different stages in its entire life.
<img src = "https://user-images.githubusercontent.com/70228962/195288096-8cf86cdf-e93e-4da1-a7fe-7710ece088f6.png">

 How can you use the test pyramid model to reduce the number of bugs that make their way into production?
The test pyramid model is a way of thinking about the different types of tests that should be used when developing software. The idea is that there should be more low-level unit tests than higher-level integration tests. This is because unit tests can be run more quickly and cheaply, and they can be used to target specific parts of the code. By having more unit tests, you can find and fix bugs before they make their way into the integration tests and eventually into production.


Q3. What is Code Coverage?
Answer:

Code coverage is a metric that determines the number of lines of code validated successfully by a testing process, which helps to analyze how software is verified in depth.


Explain the states of Bug Lifecycle.

New: When the defect or bug is logged for the first time it is said as New.
Assigned: After the tester has logged a bug, his bug is being reviewed by the tester lead and then it is assigned to the corresponding developer team.
Open: Tester logs a bug in the Open state and it remains in the open state until the developer has performed some task on that bug.
Resolved/Fixed: When a developer has resolved the bug, i.e. now the application is producing the desired output for a particular issue, then the developer changes its status to Resolved/Fixed.
Verified/Closed: When a developer has changed the status to resolved/fixed then the tester now tests the issue at its end and if it’s fixed then he changes the status of the bug to ‘Verified/Close’.
Reopen: If a tester is able to reproduce the bug again i.e. the bug still exists even after fixing by the developer, it’s status is marked as Reopen.
Not a bug/Invalid: A bug can be marked as invalid or not a bug by the developer when the reported issue is as per the functionality but is logged due to misinterpretation.
Deferred: Usually when the bug is of minimal priority for the release and if there is lack of time, in that case, those minimal priority bugs are deferred to the next release.
Cannot Reproduce: If the developer is unable to reproduce the bug at its end by following the steps as mentioned in the issue.


 What is Automation testing?

Answer: Automation testing is a testing methodology where an automation tool is used to execute the test cases suite in order to increase test coverage as well as speed to test execution. Automation testing does not require any human intervention as it executes pre-scripted tests and is capable of reporting and comparing outcomes with previous test runs.

Repeatability, ease of use, accuracy, and greater consistency are some of the advantages of Automation testing.

Some automation testing tools are listed below:

Selenium
Tellurium
Watir
SoapUI

Accessibility Testing 
Accessibility testing is the practice of ensuring your mobile and web apps are working and usable for users without and with disabilities such as vision impairment, hearing disabilities, and other physical or cognitive conditions. 

Acceptance Testing 
Acceptance testing ensures that the end-user (customers) can achieve the goals set in the business requirements, which determines whether the software is acceptable for delivery or not. It is also known as user acceptance testing (UAT).  

Black Box Testing 
Black box testing involves testing against a system where the code and paths are invisible. 

End to End Testing 
End to end testing is a technique that tests the application’s workflow from beginning to end to make sure everything functions as expected. 

Functional Testing 
Functional testing checks an application, website, or system to ensure it’s doing exactly what it’s supposed to be doing. 

Interactive Testing 
Also known as manual testing, interactive testing enables testers to create and facilitate manual tests for those who do not use automation and collect results from external tests.  

Integration Testing 
Integration testing ensures that an entire, integrated system meets a set of requirements. It is performed in an integrated hardware and software environment to ensure that the entire system functions properly.  

Load Testing 
This type of non-functional software testing process determines how the software application behaves while being accessed by multiple users simultaneously. 

Non Functional Testing 
Non functional testing verifies the readiness of a system according to nonfunctional parameters (performance, accessibility, UX, etc.)  which are never addressed by functional testing. 

Performance Testing 
Performance testing examines the speed, stability, reliability, scalability, and resource usage of a software application under a specified workload. 

Regression Testing 
Software regression testing is performed to determine if code modifications break an application or consume resources. 

Sanity Testing 
Performed after bug fixes, sanity testing determines that the bugs are fixed and that no further issues are introduced to these changes.  

Security Testing 
Security testing unveils the vulnerabilities of the system to ensure that the software system and application are free from any threats or risks. These tests aim to find any potential flaws and weaknesses in the software system that could lead to a loss of data, revenue, or reputation per employees or outsides of a company. 

Single User Performance Testing 
Single user performance testing checks that the application under test performs fine according to specified threshold without any system load. This benchmark can be then used to define a realistic threshold when the system is under load.  

Smoke Testing 
This type of software testing validates the stability of a software application, it is performed on the initial software build to ensure that the critical functions of the program are working. 

Stress Testing 
Stress testing is a software testing activity that tests beyond normal operational capacity to test the results. 

Unit Testing 
Unit testing is the process of checking small pieces of code to ensure that the individual parts of a program work properly on their own, speeding up testing strategies and reducing wasted tests. 

White Box Testing 
White box testing involves testing the product's underlying structure, architecture, and code to validate input-output flow and enhance design, usability, and security. 

What is the order of testing?
There are four main stages of testing that need to be completed before a program can be cleared for use: unit testing, integration testing, system testing, and acceptance testing.

![image](https://user-images.githubusercontent.com/70228962/195306718-fbe82030-08e1-4ac8-9f85-0d6042feb5a4.png)

What is Test Documentation?
Test documentation is documentation of artifacts created before or during the testing of software. It helps the testing team to estimate testing effort needed, test coverage, resource tracking, execution progress, etc


