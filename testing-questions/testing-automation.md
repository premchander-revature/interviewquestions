1. What’s the difference between TDD and BDD? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

| Behavior Driven Development (BDD)                                    | Test Driven Development (TDD)             |
|----------------------------------------------------------------------|-------------------------------------------|
| BDD Scenarios are derived through collaboration between team members | Implemented by developers                 |
| BDD Scenarios are written in Natural Language                        | Written in a programming language         |
| Created and maintained by the entire team                            | Created and maintained by developers      |
| Black-box testing                                                    | White-box testing                         |
| Tests the end-to-end behavior of the application                     | Tests are written for individual function |

</blockquote>
</details>
  
---

2. What is meant by BDD testing ?


![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Behavior Driven Development (BDD) Testing is used to test an application's behavior from the end user's standpoint. 
  
In BDD, test cases are written in a natural language that even non-programmers can read.
  
</blockquote>
</details>
  
---

3. What is automation testing?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Automation testing is a software testing strategy in which a tester programmatically runs the tests using a tool or a framework instead of manually going through the test cases and executing them one by one.

</blockquote>
</details>
  
---

4. What is Selenium?


![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Selenium is an open-source automated testing framework for validating web applications across multiple browsers and platforms.

</blockquote>
</details>
  
---

4. What are the Selenium suite components?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

- **Selenium Client API** - Support for writing Selenium in various languages.
- **Selenium Remote Control** - Server that allows for running web application written in those various languages.
- **Selenium Grid** - A server that can test using multiple machines running in parallel.
	- Beneficial for scaling your application across multiple browsers/OSs.
- **Selenium IDE** - Plugin used to set up testing scripts and offer record-and-playback automation functionality.
- **Selenium WebDriver** - A Serverless way to execute your scripts. The heart of Modern Selenium. Starts a browser and controls it.
	- Each type of browser has its own Selenium WebDriver.
		- chromedriver	->	Google Chrome
		- geckodriver	->	Mozilla Firefox
		- edgedriver	->	Microsoft Edge


</blockquote>
</details>
  
---

5. Can selenium be used to launch web browsers?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Yes, using selenium webdriver.

</blockquote>
</details>
  
---

6. Why do yiu need Selenium Automation Testing?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Let's consider a  scenario: Checking whether the web app’s signup page (www.example.com/signup) validates input strings and registers a user successfully.

Assume that the signup page has these input fields—username, email address, and password. 

As a manual tester, we need to follow these steps:

1. Enter the URL in the address bar (www.example.com/signup)
2. Enter an invalid string in each input field (email, username, and password)
3. Check whether the input strings were validated against corresponding regexes and any pre-existing values in the database
4. Enter _valid_ strings in each input field; click Sign Up
5. Check whether _Welcome, {username}_ page showed up
6. Check whether the system database created a new userID for _{username}_
7. Mark the test _passed_ if it did, _failed_ if the signup feature broke anywhere during the test.

Depending on the number of manual testers (and thoroughness of test cases), it may take anywhere between hours to weeks to be sure that the web app is fully functional.

Modern developers and product teams don’t have that kind of time to allot for testing, but they can’t set aside exhaustive testing in a hurry to release either. 

This is why we go for automation testing with Selenium.

</blockquote>
</details>
  
---



