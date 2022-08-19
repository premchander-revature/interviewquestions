## Core Spring 

1. What is Dependency Injection & Where all Spring framework can be used?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
  
Dependency injection is basically providing the instance variables (referred do as dependencies) that an object needs, instead of having it constructed by the class of that object itself. Spring framework can be used to build Java CUI, GUI, Web, Distributed, Enterprise Applications, as all application types are candidate for Dependency injection.
  
**Explanation**<br>  There are scenarios where one java class comprises of dependencies i.e. object of another class. This is particularly called as Has-A relationship in java world. Whenever in any java application you have one or more dependencies which you don’t want to manage on your own rather want to delegate it to some third-party framework that is right place where Spring framework can be leveraged. The wrong myth for Spring is, it is only used for enterprise application but in reality, it can be used in any type of application as far as you have dependencies in your code. Hence Spring framework can be used in any Core Java, Web, Distributed, Web Services as well as Android application as applicable.

``` java
  
public class Laptop {
	private String modelName;
	private double price;
	private Processor processor;
	// Constructor auto-generated constructor stub
	// Getter, Setter auto-generated stub
}

public class Processor {
	private String modelName;
	private String cacheMemory;
	private double price;
	// Constructor auto-generated constructor stub
	// Getter, Setter auto-generated stub
}

public class Intel extends Processor {
	private String numberOfCores;
	// Constructor auto-generated constructor stub
	// Getter, Setter auto-generated stub
}

public class Amd extends Processor {
	private boolean graphicsAcceleration;
	// Constructor auto-generated constructor stub
	// Getter, Setter auto-generated stub
}
```
 </blockqoute> 
</details>

---
  
2. What is IoC and Dependency Injection in Spring?
  
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
  
 Inversion of control is a generic term and implemented in several ways (events, delegates, service locator & Dependency Injection). DI is a subtype of IOC and is implemented by constructor injection, setter injection or method injection.
  
**Explanation**<br> **IoC** which stands for **Inversion of Control** is also known as **Dependency Injection (DI)** usually referred as **Spring IoC/DI**. Inversion of Control is a principle in software engineering which transfers the control of objects or portions of a program to a container or framework. In contrast with traditional programming, in which our custom code makes calls to a library, IoC enables a framework to take control of the flow of a program and make calls to our custom code. It is a process whereby objects define their dependencies (that is, the other objects they work with) through constructor arguments (called Constructor based DI) or properties that are set on the object instance after it is constructed (called Setter based DI). The container then injects those dependencies when it creates the bean. This process is fundamentally the inverse (hence the name, Inversion of Control) of the bean itself controlling the instantiation or location of its dependencies.

  **Note:** Remember Dependency Injection (DI) is broader term used and supported by many frameworks including frontend framework like Angular.  In Angular we have Services that share data between various components are also configured using DI.
  </blockqoute> 
</details>
  
 ---
  
 
3. What is IoC Container or DI Container? (What is the role of an IoC container?)

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
  
In spring context both IoC & DI containers are the same. In Spring the business components are called as Beans. The IoC container manages the lifecycle of Beans.

**Explanation**<br>
The terms Dependency Injection (DI) & Inversion of Control (IoC) are generally used interchangeably, hence some people say IoC Container and some people say DI container but both terms indicate the same thing. The IoC container that is also known as a DI Container is a framework for implementing automatic dependency injection very effectively. It manages the complete object creation and its lifecycle, as well as it also injects the dependencies into the classes. In the Spring framework, the interface **ApplicationContext** represents the IoC container. The Spring container is responsible for instantiating, configuring and assembling objects known as beans, as well as managing their life cycles. The Spring framework provides several implementations of the **ApplicationContext** interface: **ClassPathXmlApplicationContext** and **FileSystemXmlApplicationContext** for standalone applications, and **WebApplicationContext** for web applications.
