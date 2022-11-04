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

7. List the steps to perform a test through Selenium?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

1. Download browser drivers
2. Create a WebDriver instance.
3. Navigate to a webpage.
4. Locate a web element on the webpage via locators in selenium.
5. Perform one or more user actions on the element.
6. Preload the expected output/browser response to the action.
7. Run test.
8. Record results and compare results from them to the expected output.
9. Close the WebDriver

</blockquote>
</details>
  
---

8. How do you navigate to a particular webpage URL?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

To navigate to a particular webpage URL, one can use either of the following commands:

- Using get method: 
	
```java
driver.get (“https://www.example.com”) ;
```	
	
- Using the navigate method

```java
driver.navigate().to("https://www.example.com/signup");
```
	
</blockquote>
</details>
  
---

9. How can I move to a page in the browser history in selenium?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

The forward command navigates the browser forward by one page recorded in the browsing history.

```java
driver.navigate().forward();
```
	
</blockquote>
</details>
  
---

10. How can I go back to the previous page in selenium?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

The back command instructs the browser to redirect to the immediate previous webpage.

```java
driver.navigate().back();
```
	
</blockquote>
</details>
  
---

11. How can I reload a page using selenium?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

The Refresh command instructs the browser to reload or refresh the current web page.

```java
driver.navigate().refresh();
```

</blockquote>
</details>
  
---

12. What are Locators in Selenium? List the types of locators.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

A locator enables testers to select an HTML DOM element to act on. Some of the different locators are:

|        Method        |                        Syntax                       |                  Description                 |
|:--------------------:|:---------------------------------------------------:|:--------------------------------------------:|
| By ID                | driver.findElement(By.id (<element ID>))            | Locates an element using the ID attribute    |
| By name              | driver.findElement(By.name (<element name>))        | Locates an element using the Name attribute  |
| By class name        | driver.findElement(By.className (<element class>))  | Locates an element using the Class attribute |
| By tag name          | driver.findElement(By.tagName (<htmltagname>))      | Locates an element using the HTML tag        |
| By link text         | driver.findElement(By.linkText (<linktext>))        | Locates a link using link text               |
| By partial link text | driver.findElement(By.partialLinkText (<linktext>)) | Locates a link using the link's partial text |
| By CSS               | driver.findElement(By.cssSelector (<css selector>)) | Locates an element using the CSS selector    |
| By XPath             | driver.findElement(By.xpath (<xpath>))              | Locates an element using XPath query         |

</blockquote>
</details>
  
---

13. Consider the following form and tell me how we can locate the input elements.
```html
<form id="loginForm">
	<input name="name" type="text" value="Name" />
	<input name="email" type="text" value="Email" />
</form>
```

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Using the `driver.findElement(By.name (<element name>))` method, we can locate the `name` and `email` form element.
	
```java
email_input = driver.findElement(By.name("email"))
name_input = driver.findElement(By.name("name"))
``` 	

</blockquote>
</details>
  
---

14. Consider the following form and tell me how we can locate the input elements.
```html
<form id="loginForm">
	<input name="name" type="text" value="First Name" />
	<input name="name" type="text" value="Last Name" />
</form>
```

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

If we can locate by name, we able to only locate first name not the last name. Also, we can't locate first name and last name by by ID or class. So, we can locate these elements through its XML path.  
	
We will use the `driver.findElement(By.xpath (<xpath>))` method to locate an appropriate element in the document. 
	
The following code first searches for a form with the ID login form and then selects the form’s first and second input elements as the first and last names.

```java
first_name = driver.findElement(By.xpath ("//form[@id='loginForm']/input[1]"))
last_name = driver.findElement(By.xpath ("//form[@id='loginForm']/input[2]"))
```

</blockquote>
</details>
  
---

15. How can I get all the elements in the HTML DOM?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

The `findElementsBy()` method helps in finding multiple elements in the DOM structure.

For example, to find all input elements of a form with ID loginForm, we use: 
	
```java
List<WebElement> inputs = driver.findElementsBy(By.id("loginForm"));
```
	
</blockquote>
</details>
  
---

16. What is HTML Source?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

HTML Source refers to the HTML code underlying a certain web element on a web page.

</blockquote>
</details>
  
---

17. What is a Web Element?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

- Anything that appears on a web page is a web element. Also, web elements mean the tags within the web page’s HTML code.
- Web element refers to text boxes, checkboxes, buttons, or any other fields that display or require data from the user. Such elements usually have unique identifiers, such as ID, name, or unique classes. 

</blockquote>
</details>
  
---

18. `FindElement()` vs `FindElements()`

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

| Find Element                                                                                      | Find Elements                                                                    |
|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| Returns the first most web element if there are multiple web elements found with the same locator | Returns a list of web elements                                                   |
| Throws exception NoSuchElementException if there are no elements matching the locator strategy    | Returns an empty list if there are no web elements matching the locator strategy |
| Find element by XPath will only find one web element                                              | It will find a collection of elements whose match the locator strategy.          |
| Not Applicable                                                                                    | Each Web element is indexed with a number starting from 0 just like an array     |
| Example: driver.findElement(By.id("no"))                                                          | Example: List elements = driver.findElements(By.name("name"));                   |

</blockquote>
</details>
  
---
	
19. What is XPath in Selenium?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

XPath, also known as XML Path, used to locate any element in a web page using its tag name, ID, CSS class, and so on.
	
The basic format of XPath in Selenium is explained below.
```
XPath = //tagname[@Attribute=’Value’]
```
	
Here,

- `//`: denotes the current node
- `tagname`: denotes the tagname of the current node
- `@`: is the Select attribute
- `Attribute`: denotes the attribute of the node
- `Value`: denotes the value of the chosen attribute

</blockquote>
</details>
  
---
	
20. What are the types of XPath in Selenium?
	
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

There are two types of XPath in Selenium.

1. **Absolute XPath** 
	- It starts with a single slash `/`
	- Provides the entire path starting from the root node
	- Example: `/html//div/div/div/div[1]/div/a/img`
2. **Relative XPath** 
	- It starts with double slash `\\`
	- Here XPath expression starts from the middle of the DOM structure denoting the current node.
	- Example: `//img[@alt='LambdaTest']`

</blockquote>
</details>
  
---	
