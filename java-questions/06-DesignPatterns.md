1. What is stateless?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
When we implement the stateless design pattern, we create classes and objects that do not retain state changes. In this approach, each use of the object, as an example, uses the object in its organic form. In our context, state refers to the values of the object's variables. So, there is no definitive list of states. The state of an object is specific to a moment in time. 
 
</blockquote>
</details>

--- 

2. What is DAO?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
Data Access Object Pattern is used to isolate low-level data accessing API or actions from high-level business services. Following are the components in the DAO Pattern.

Data Access Object Interface:DAO interface describes the standard actions to be performed on a model objects.

Data Access Object concrete class:This class implements a DAO interface. This class is accountable to get data from a data source which can be Xml/database or any other storage mechanism.

Model Object or Value Object:This object is a plain old java object containing get/set methods to store data retrieved using DAO class.
</blockquote>
</details>

--- 

3. What is a singleton?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object. This is helpful usually when a single object is required to coordinate actions across a system.
 
</blockquote>
</details>

--- 
