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
</details>

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

16. Do you know what are the various forms of writing lambda expressions?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- () -> expression
- (parameters) -> expression
- (parameters) -> { multiple statements}

</blockquote>
</details>

---

17. What do you understand by @Functional Interface annotation in Java 8?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- @Functional interface , if used will force the compiler to check whether the given interface has single-abstract method or not.
- If not, compiler will throw error "Unexpected @FunctionalInterface annotation"

</blockquote>
</details>

---

18. How do you create a custom annotation in Java?

![Complex](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Complex%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- Example :
@Retention(RetentionPolicy.RUNTIME)
@Target(ElementType.Type)
public @interface ByteProgramming
{
    String username() default "ByteProgramming";

}
@ByteProgramming(username="Byte")

</blockquote>
</details>

---

19. How to avoid NullPointer exception in Java 8?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- Java 8 provides concept of Optionals
- Optionals can be used to avoid NullPointer Exception

- Ex: String value=null;
     * Optional<String> value=Optional.empty();
</blockquote>
</details>

---

20. What are the functional interfaces you have used in your project, introduced in Java 8?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- Functional interfaces like Function like Function, Consumer, Supplier, Predicate
- All these are part of java.util.function package.

</blockquote>
</details>

---

21. How would you convert object of type Iterable to stream ?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- Example
- * StreamSupport.stream(iterable.spliterator(),false).forEach( stud -> { System.out.println(stud); });

</blockquote>
</details>

---

22.  How to come overcome, multiple inheritance problem in Java 8 ?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

Override the default method in the implementation class
Altogether provide new implementation or
Invoke either one of the default method using super keyword
For example, <interfaceName>.super.<defaultMethodName>

</blockquote>
</details>

---

23. What happens, if a class implements 2 interfaces having exactly same method with same signature (consider one as default and another abstract) ?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- Compilation fails with error saying conflicting method.
- Compile-time error: The default method displayDefaultMethod() inherited from DemoInterfaceA conflicts with another method inherited from DemoInterfaceB
- To overcome this error, override this conflicting method and provide new implementation or invoke default method’s implementation using super keyword

</blockquote>
</details>

---

24. How can we resolve ambiguity problem in Java 8 while implementing multiple Interfaces ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

To resolve ambiguity problem in Java 8, override the conflicting method.
Now, if we want to invoke default method from any of the interfaces then call using super keyword
For example, <interfaceName>.super.<defaultMethodName>

</blockquote>
</details>

---

25. What is the purpose of join() method introduced in Java 8 ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

Java 8 added overloaded static join methods that join multiple strings into a single string.

</blockquote>
</details>

---

26. What is the use of the String::ValueOf expression in Java 8?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

String::ValueOf is a simple static method referencing the valueOf method, belonging to the class 
‘String.’

</blockquote>
</details>

---

27. What is the meaning of method reference in Java 8?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

Method references are used in Java 8 to refer to methods of functional interfaces. It can be considered as a short-code version of using a lambda expression.

The following is the expression for a method reference:

    Class::methodname
</blockquote>
</details>

---

28. What is the easiest way to print the current date and time using the new APIs in Java 8?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

The ‘now’ method, which is a part of LocalDate, can be used to get the current date as shown below:

LocalDate currentDate = LocalDate.now();
System.out.println(currentDate);

Similarly, it can also be used to get the current time:

LocalTime currentTime = LocalTime.now();
System.out.println(currentTime);

</blockquote>
</details>

---

29. Differentiate between intermediate and terminal operations in Java 8.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

*** Intermediate Operation ***
Used for the transition to a new state	
Lazy execution of code, i.e., code is not executed as soon as it is encountered	Not lazy; 

*** Terminal Operation ***
Used to end the process under execution
code is immediately executed upon encounter

</blockquote>
</details>

---
30. Can the following piece of code compile successfully?

<blockquote>
@FunctionalInterface<br>
public interface Function2<T, U, V> {<br>
public V apply(T t, U u);<br>
default void count() {<br>
    // increment counter<br>
}<br>
}<br>
</blockquote>

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

Yes, the code can compile and execute without any errors. It uses functional interface specifications when the single abstract method is being defined.

</blockquote>
</details>

---

31. What is the code to sort strings using the Java 8 lambda expression?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

The below piece of code sorts strings using the lambda expression:

//Sorting using Java 8 lambda expression

private void sortUsingJava8(List<String> names) {

Collections.sort(names, (s1, s2) -> s1.compareTo(s2));

}
</blockquote>
</details>

---

32. Is it possible to call a static method of any interface in a class using Java 8?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

Yes, it is possible to call a static method in a class by making use of the name as shown below:

interface Student {
static void Present() {
System.out.println("Student is there!");
}
}

class Associates implements Student {
public void print() {
Student.Present();
}

</blockquote>
</details>

---

33. Do you knoq how the random keyword in Java 8 works?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

The random keyword, as the name suggests, is used to generate random values for computations and operations in Java 8.

The following piece of code is used to print out 20 random numbers using the forEach loop:

Random random = new Random();
random.ints().limit(20).forEach(System.out::println);

</blockquote>
</details>

---

34. What are collectors in Java 8?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

Collectors are mainly used to combine the final result after the processing of elements in a stream. They are used to return lists or strings.

</blockquote>
</details>

---

35. What is the easiest way to print the sum of all of the numbers present in a list using Java 8?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

In Java 8, the following code is used to print the sum of all of the numbers that are present in a list:

List<Integer> numbers = Arrays.asList(5, 4, 10, 12, 87, 33, 75);
IntSummaryStatistics stats = integers.stream().mapToInt((x) −> x).summaryStatistics();
System.out.println("Sum of all numbers : " + stats.getSum());

</blockquote>
</details>

---

36. When is an ideal situation to use the Stream API in Java 8?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

- The Stream API in Java 8 can be effectively used if the Java project calls for the following operations:

 * Perform database operations
 * Execute operations lazily
 * Write functional-style programming
 * Perform parallel processing
 * Use pipeline operations
 * Use internal iteration

</blockquote>
</details>

---

37. Can you tell me about supplier in Java 8?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>
A supplier is a simple functional interface in Java 8 that does not take in any argument. It is used as an assignment target when making use of lambda expressions.

</blockquote>
</details>

---

38. Do you know about predicate in Java 8 ?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

Just like a predicate, a consumer is a single argument functional interface present in Java 8. However, the consumer does not return any value and can be used for lambda expressions.

</blockquote>
</details>

---

39. Can you name the common types of functional interfaces in the standard library?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>

There are many functional interface types in the standard library, and some of them are as follows:

- BiFuction
- BinaryOperator
- Consumer
- Predicate
- Supplier
- UnaryOperator

</blockquote>
</details>

---

40. Can you give examples of intermediate operations in Java 8?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>
<blockquote>
The examples that are widely used in intermediate operations are:

- Distinct()
- Limit(long n)
- Filter(Predicate)
- Map(Function)
- skip(long n)

</blockquote>
</details>

---

