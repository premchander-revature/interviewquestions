1. Difference between method and function

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
- Method and a function are the **same, with different terms**.
- A method is a **function that belongs to a class**.
- A function is a group of reusable code which can be called anywhere in your program.

</blockquote>
</details>

--- 

2. Tell us about OOPs

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>

- **O**bject **O**riented **P**rogramming is a programming paradigm/model which revolves around the concept of **Objects**. 
- Objects can be considered as real-world instances of entities like class, that have **characteristics** and **behaviors**

**For example**, if we consider a car, then based on the OOPs model:

- Class: A specific car model, such as Audi A4, BMW I8, Maruti Suzuki Vitara Brezza, etc.
- Object: A specific car of any model, like the car you own
- Characteristics: What is the color of your car? What is the model of your car? etc
- Behavior: How to start the car? How to change the gear of the car? etc.

Characteristics are also known as data, attributes, or properties, and Behaviours are also known as the functions, procedures or methods, in the programming language.

</blockquote>
</details>

--- 

3. What are the pillars of OOP?
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>

The Four Pillars of Object-Oriented Programming are
- Abstraction
- Encapsulation
- Inheritance
- Polymorphism

</blockquote>
</details>

--- 

3. What is polymorphism?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
- The word poly means many and morphs means forms, So polymorphism means many forms.
- It's an ablility of an object to exhibit more than one form

For example: A man at the same time is a father, a husband, an employee. So the same person possesses different behavior in different situations. This is called polymorphism. 

</blockquote>
</details>

--- 

4. What is method overloading?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
<blockquote>
 
- Method Overloading is a feature that allows a class to have more than one method with the same name, but with different parameters.
- It is also known as Compile-time Polymorphism or Static Polymorphism 

**For example**: 
```java
public class SquaringDemo {
	
	public void square(int n) {
		System.out.println("Method with int argument called: " + n*n);
	}
	public void square(double n) {
		System.out.println("Method with double argument called: " +n*n);
	}
	public void square(float n) {
		System.out.println("Method with float argument called: " + n*n);
	}

	public static void main(String[] args) {
	  SquaringDemo obj = new SquaringDemo();
	  obj.square(4);
	  obj.square(4.567);
	  obj.square(4.567f);
	}
	/*Output:
	 * Method with int argument called: 16
	 * Method with double argument called: 20.857489
	 * Method with float argument called: 20.857489
	 */
}
```

</blockquote>
</details>

--- 

5. What is method overriding?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>

If there is a same method is defined in both the superclass and the subclass, then the subclass's method overrides the superclass's method. This is known as method overriding. It's also called as dynamic polymorphism or run-time polymorphism.

For example,
```java
class Animal {
   public void makeSound() {
      System.out.println("I am an animal.");
   }
}

class Dog extends Animal {
   @Override
   public void makeSound() {
      System.out.println("I am a dog!!, woof woof");
   }
}

class Cat extends Animal{
	@Override
	   public void makeSound() {
	      System.out.println("I am a cat!!, meow meow");
	   }
}
```
 
 
</blockquote>
</details>

--- 

6. Explain encapsulation

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>

Encapsulation is the way of binding the data (variables) and code acting on the data (methods) together as a single unit.  

For example, in a company, they are different sections like the accounts section, finance section, sales section etc. Consider a situation, a person from finance section needs all the data about sales in a particular month. In this case, he is not allowed to directly access the data of sales section. He will first have to contact some other officer in the sales section and then request him to give the particular data. This is what encapsulation is. 

In encapsulation, the variables of a class will be hidden from other classes, and can be accessed only through the methods of their current class. Therefore, it is also known as data hiding.

</blockquote>
</details>

--- 

7. What is an abstract class?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

8. Brief us on interfaces

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

9. Difference between abstract classes and interfaces

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

10. What is Abstraction?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

11. What is inheritance? (or) Brief us on inheritance

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

11. Describe abstract in OOP (or) What does Abstraction do?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

12. Brief us on encapsulation and access modifiers

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

13. How many constructors you used in java?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

14. Can you do static overriding?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

15. What are the types of Inheritance?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

16. When do you use Abstract Class and Interfaces?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

17. Brief us on the types of Polymorphism

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

18. Can the main method be overridden?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

19. What are Constructors?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

20. What is a class? What is an object?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

21. What is the benefit of inheritance?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

22. Can we implement multiple inheritances in Java?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

24. Can you change the scope of a method or class using inheritance?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

25. What are some of the advantages of inheritance?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

26. What are the benefits of abstraction?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

27. What is the difference between class and object?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Show Answer</b></summary>
  
<blockquote>
 
 
</blockquote>
</details>

--- 

