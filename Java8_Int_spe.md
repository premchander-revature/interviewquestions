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

- No, for defining default method inside interface “default” keyword is must and it should prefix method declaration
- Without prefixing default keyword results in compilation error
- Compile-time error: Abstract methods do not specify a body
- Reason: without default keyword, compiler consider it as abstract method and as said abstract methods doesn’t have body

</details>
