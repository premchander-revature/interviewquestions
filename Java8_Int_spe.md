## Technical
1. In java 8 how can I filter a collection using the stream?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

- It provides a method filter() to filter stream elements on the basis of given predicate. 
- This method take predicate as an argument and returns a stream of consisting of resulted elements.

</details>

---

2. Is it ok to define default methods in Java 8 without “default” keyword inside interface ?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- No, for defining default method inside interface “default” keyword is must and it should prefix method declaration
- Without prefixing default keyword results in compilation error
- Compile-time error: Abstract methods do not specify a body
- Reason: without default keyword, compiler consider it as abstract method and as said abstract methods doesn’t have body
</blockquote>
</details>

---

3. What actual advantage does Java 8 bring ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- code is more concise and readable
- more reusable,testable and maintable
- user can write parallel code
- user can write database like operations
</blockquote>
</details>

---

4. What enhancements have been done to JDK?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- Unitl Java 7, JVM used an area called PermGen to store classes. IT gor removed in Java 8 and replaced by MetaSpace.
- Major advantage of MetaSpace over permgen: Permgen was fixed in term of maximum size and cannot grow dynamically but Metaspace can grow dynamically and do not have any size constraint.

</blockquote>
</details>

---

5. What changes have been done to HashMap in Java 8?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

Buckets containing a large number of colliding keys will store their entries in a balanced tree instead of a linked list after certain threshold is reached.

</blockquote>
</details>

---

6. How lambda expressions and functional interface are related?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

Lambda expressions can only be applied to abstract method of functional interface.

</blockquote>
</details>

---

7. What is your underatnding about stream pipelining?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

Stream pipelining is the process of chaining different operations together. It accomplishes this function by dividing stream operations into two categories, intermediate operation and terminal operations.

</blockquote>
</details>

---

8. Can you create your own functional interface?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

Yes, we can. create our own functional interface.
</blockquote>
<details>
---

9. What will happen if i am using a Functional interface and if i define multiple abstract methods inside that interface?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

It will throw a compiletime error.

</blockquote>
</details>

---

10. Why default methods needed in the inteface?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

Default methods let us to add new functionality tto the libraries interfaces and ensure binary compatability with older code written for the imterfaces.

</blockquote>
</details>

---

11. What is the behaviout of findFirst() method in Java 8  streams?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

The findFirst() method returns the first element of a stream or an empty Optional. If the stream has no encounter order, any element is returned, as it's ambiguous which is the first one anyway.

</blockquote>
</details>

---

12. What is the behaviout of findAny() method in Java 8  streams?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

The findAny() method returns any element of the stream - much like findFirst() with no encounter order.

</blockquote>
</details>

---

13. When to use findAny() method in Java 8 streams?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

There are instances where you have a stream, but you only want to select a random element; as long as it meets certain conditions and the operation itself takes the shortest time possible.

</blockquote>
</details>

---

14. What do you mean by stream ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- Streams are just sequence of data from a source.
- With Java 8, we can do manipulation on data using stream API.
- Example: Youtube

</blockquote>
</details>

---

15. Can you tell me difference between CollectionAPI and Stream API?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- Collection API is used for storing data in different kinds of data structures.
- Stream API is used for computation of data on a large set of objects.
- With Collection API we can store a finite number of elements in a data structure.
- With Stream API, we can handle streams of data that can contain infinite number of elements.
- Collection API constructs objects in an eager manner.
- Stream API creates objects in a lazy manner.
- Multiple consumption: Most of the Collection APIs support iteration and consumption of elements multiple times.
- With Stream API we can consume or iterate elements only once.

</blockquote>
</details>

---

