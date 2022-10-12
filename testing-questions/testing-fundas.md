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

<img src = "https://user-images.githubusercontent.com/70228962/195267678-4f17c0c7-71b7-4210-8ae9-7d1e4cc15af9.png" height = "300"/>

</blockquote>
</details>
  
---

What is meant by entry criteria and exit criteria?
Entry Criteria: Entry Criteria are a set of conditions that need to be satisfied in order to begin the test.
Exit Criteria: Exit Criteria are a set of conditions that need to be satisfied in order to end the test.

What is the purpose of the test closure phase?
Test closure activities have several purposes, such as to:

Make sure testing is completed.
Gather and submit test artifacts.
Hold retrospective meetings to review previous information and improve.

What is the difference between SDLC and STLC?

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

<img src = "https://user-images.githubusercontent.com/70228962/195288096-8cf86cdf-e93e-4da1-a7fe-7710ece088f6.png">



