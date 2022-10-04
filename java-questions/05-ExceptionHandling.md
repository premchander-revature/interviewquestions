1. Brief us on Exception handling

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
Exception is something which can be handled and can continue the same flow of execution.
Exception handling will help you to handle the exceptions which has been raised and terminate normally with the proper communication to the end user, where such app which handles all the abnormal status normally its the app which is sold highest in any market.

 
</blockquote>
</details>

--- 

2. What is the difference between Throw and Throws?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
throws is used to throw multpile exceptions at the method level to  calling the method and use it to force the programmer who is creating the object for that
method will handle it.
throw is used to create the exception object of our own to throw our own customised exception with our own customised message.

 
</blockquote>
</details>

--- 

3. How to handle class not found exception

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
Java ClassNotFoundException occurs when the application tries to load a class but Classloader is not able to find it in the classpath.
ClassNotFoundException is a checked exception, so it has to be catch or thrown to the caller.ClassNotFoundException always occurs at runtime because we are indirectly loading the class using Classloader.
 
</blockquote>
</details>

--- 

4. Brief us on the keywords - final, finally & static 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 final is the keyword and access modifier which is used to apply restrictions on a class, method or variable.
 finally is the block in Java Exception Handling to execute the important code whether the exception occurs or not.
 static keyword is used to create a Class level variable in java. static variables and methods are part of the class, not the instances of the class.
 
</blockquote>
</details>

--- 

5. Brief us on Exceptions

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
An exception is an unexpected event that occurs during program execution. It affects the flow of the program instructions which can cause the program to terminate abnormally.
  
An exception can occur for many reasons. Some of them are:
Invalid user input
Device failure
Loss of network connection
 
</blockquote>
</details>

--- 

6. Brief us on Errors

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
Errors represent irrecoverable conditions such as Java virtual machine (JVM) running out of memory, memory leaks, stack overflow errors, library incompatibility, infinite recursion, etc.Errors are usually beyond the control of the programmer and we should not try to handle errors.
 
</blockquote>
</details>

--- 

7. What is the difference between Final and finally?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
Final is a keyword and it can be used to mark a variable "unchangeable" . Actually, it is used to apply restrictions on class, method and variable. Final class can't be inherited, final method can't be overridden and final variable value can't be changed.
Finally is a code block. It is used with try-catch block for handling exception. finally code block will be executed whether exception is handled or not
 
</blockquote>
</details>

--- 

8. Tell us about the different kinds of exceptions. What are some examples of checked and unchecked exceptions?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 There are 2 types of exceptions
  a)Checked Exception(java.lang.Exception) -> This exception forces the progarmmer to handle it at the compile time itself, until the programmer handles it, compiler wont allow to run.
some of Checked exceptions are FileNotFoundException, ClassNotFoundException,MethodNotFoundException, SQLException and more.
  b)Unchecked Exceptions(java.lang.RuntimeException) -> These exceptions are part of java.lang.RunTimeException which occurs at a run time, it is upto programmer whether he wants to handle this or not, if he doesnt handle it, it will lead to abnormal termination.
 few unchecked exceptionsare:ArithmeticException,NullPointerException,ConcurrentModificationException,ArrayIndexOutOfBoundException.
 
</blockquote>
</details>

--- 


