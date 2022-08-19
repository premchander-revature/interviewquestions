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
**Note:** Laptop class having Processor dependency
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
  </blockqoute> 
</details>
  
 ---
 
 4. Any DI frameworks apart from Spring?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
	
Libraries and Frameworks that implement DI
- Spring (Java)
- Google Guice (Java)
- Dagger (Java and Android)
- Castle Windsor (.NET)
- Unity(.NET)
  </blockqoute> 
</details>
  
 ---

5. What are the types of dependency injection in Spring?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
	
Dependency Injection in Spring can be done through **Constructors, Setters or Fields**.
	
**Explanation:** Lets understand with example:
``` java
public class TextEditor {
	private Validator;
	  public TextEditor(Validator validator) {
	    this.validator = validator;
	  }
	// Constructor auto-generated constructor stub
	// Getter, Setter auto-generated stub
}

public class GrammerValidator extends Validator {
	// Constructor auto-generated constructor stub
	// Getter, Setter auto-generated stub
}
```
**Note:** Class TextEditor having Validator dependency
	
**Constructor-Based Dependency Injection**<br>  In the case of constructor-based dependency injection, the DI is accomplished by the container invoking a constructor with a number of arguments, each representing a dependency.<br>
Spring resolves each argument primarily by type, followed by name of the attribute, and index for disambiguation. 

``` java
//Annotation Configuration:
@Configuration
public class AppConfig {
	@Bean
	public Validator grammerValidator() {
		return new GrammerValidator();
	}

	@Bean
	public TextEditor textEditor() {
		return new TextEditor(grammerValidator());
	}
}
//Or
//XML Configuration:
<bean id = "grammerValidator"class="com.revature.model.GrammerValidator"/>
<bean id="textEditor"class="com.revature.model.TextEditor">
	<constructor-arg type="Validator"index="0"name="validator"ref="grammerValidator"/>
</bean>
```
	
**Setter-Based Dependency Injection**<br> In the case of setter-based dependency injection, the container will call setter methods of our class after invoking a no-argument constructor (or no-argument static factory method) to instantiate the bean. We can combine constructor-based and setter-based types of injection for the same bean. The Spring documentation recommends using constructor-based injection for mandatory dependencies, and setter-based injection for optional ones.

``` java
//Annotation Configuration:
@Configuration
public class AppConfig {
	@Bean
	public TextEditor textEditor() {
		TextEditor = new TextEditor();
		textEditor.setValidator(grammerValidator());
		return textEditor;
	}

	@Bean
	public Validator grammerValidator() {
		return new GrammerValidator();
	}
}
//Or 
//XML Configuration:
<bean id="grammerValidator" class="com.revature.model.GrammerValidator"/> 
<bean id="textEditor" class="com.revature.model.TextEditor"> 
  <property name="validator" ref="grammerValidator"/>
</bean>
```
	
**Field-Based Dependency Injection**<br>
In the case of setter-based dependency injection, we inject the dependencies by marking them with **@Autowired** annotation.<br>
This approach might look simpler and cleaner, but it has a few drawbacks such as:
-	This method uses reflection to inject the dependencies, which is costlier than constructor-based or setter-based injection.
-	It's really easy to keep adding multiple dependencies using this approach. If we were using constructor injection, having multiple arguments would make us think that the class does more than one thing, which can violate the Single Responsibility Principle.
	
``` java
//Annotation Configuration:
//While constructing the TextEditor object, 
//if there's no constructor or setter method to inject the Validator bean, 
//the container will use reflection to inject Validator into TextEditor.

public class TextEditor {
	@Autowired
  private Validator;
}

//Or
//XML Configuration:

<bean id="grammerValidator" class="com.revature.model.GrammerValidator" /> 
<bean id="textEditor" class="com.revature.model.TextEditor" autowire="byType"/>
<bean id="textEditor" class="com.revature.model.TextEditor" autowire="byName"/>
```
When using XML-based configuration metadata, we can specify the **autowire** mode for a bean definition with the autowire attribute of the <bean/> element. The autowiring functionality has four modes. There are four modes of autowiring a bean using an XML configuration:
1.	**no**: The default value - this means no autowiring is used for the bean and we have to explicitly name the dependencies. The bean references must be defined by **ref** elements.
2.	**byName**: Autowiring by property name. Spring looks for a bean with the same name as the property that needs to be autowired.
3.	**byType**: Lets a property be autowired if exactly one bean of the property type exists in the container. If more than one exists, a fatal exception is thrown, which indicates that you may not use byType autowiring for that bean. If there are no matching beans, nothing happens (the property is not set).
4.	**constructor**: Analogous to byType but applies to constructor arguments. If there is not exactly one bean of the constructor argument type in the container, a fatal error is raised.
  </blockqoute> 
</details>
	
---
	
6. What are the bean scopes?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
	
The scope of a bean defines the life cycle and visibility of that bean in the contexts we use it. 
**Explanation**<br> You can control not only the various dependencies and configuration values that are to be plugged into an object that is created from a particular bean definition but also control the scope of the objects created from a particular bean definition. The latest version of the Spring framework defines 6 types of scopes:
1.	**singleton**: (Default) Scopes a single bean definition to a single object instance for each Spring IoC container. When we define a bean with the singleton scope, the container creates a single instance of that bean; all requests for that bean name will return the same object, which is cached. Any modifications to the object will be reflected in all references to the bean. This scope is the default value if no other scope is specified.
2.	**prototype**: Scopes a single bean definition to any number of object instances.
A bean with the prototype scope will return a different instance every time it is requested from the container. The client code must clean up prototype-scoped objects and release expensive resources that the prototype bean(s) are holding. To get the Spring container to release resources held by prototype-scoped beans, try using a custom bean post-processor, which holds a reference to beans that need to be cleaned up.
3.	**request**: Scopes a single bean definition to the lifecycle of a single HTTP request. That is, each HTTP request has its own instance of a bean created off the back of a single bean definition. Only valid in the context of a web-aware Spring **ApplicationContext**.
4.	**session**: Scopes a single bean definition to the lifecycle of an HTTP Session. Only valid in the context of a web-aware Spring ApplicationContext.
5.	**application**: Scopes a single bean definition to the lifecycle of a **ServletContext**. Only valid in the context of a web-aware Spring **ApplicationContext**.
6.	**websocket**: Scopes a single bean definition to the lifecycle of a **WebSocket**. Only valid in the context of a web-aware Spring **ApplicationContext**.

**Singleton Scoped Bean Example**
``` java
@Bean
@Scope("singleton")
//or
//@Scope(value = ConfigurableBeanFactory.SCOPE_SINGLETON)
public Laptop myLaptop() {
    return new Laptop();
}
```
![image](https://user-images.githubusercontent.com/99252558/185595446-87b66f4d-773e-4dcc-a94f-4aedfc1b79f4.png)

**Prototype Scoped Bean Example**

``` java
@Bean
@Scope("prototype")
//or
//@Scope(value = ConfigurableBeanFactory.SCOPE_PROTOTYPE)
public Laptop myLaptop() {
    return new Laptop();
}
```
![image](https://user-images.githubusercontent.com/99252558/185595878-948d15c0-3769-4d4e-9d0d-2c9467ee1ff8.png)
	
**Note**: Additional **Custom Scopes** can also be created and configured using a **CustomScopeConfigurer**. An example would be the **flow scope** added by Spring Webflow. In most cases, you may only deal with the Spring’s core scope i.e., **singleton** and **prototype**.
</blockqoute> 
</details>

---

7. What are Advantages & Disadvantages of DI?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>

The process of injecting and converting coupled or dependent objects into decoupled or independent objects is called Dependency Injection. It is a process that allows concurrent and or independent development. Through dependency injection, two developers can independently develop classes that use each other, while only needing to know the interface the classes will communicate through. Moreover, dependency injection decreases coupling between classes and its dependency. 

**Advantages of Dependency Injection:**
1.	Dependency injection allows a client the flexibility of being configurable.
2.	Classes are more modular, as they depend only on the interface of passed-in dependencies. Class behavior can be changed by swapping out a new component.
3.	Centralized configuration can be used to externalize a system's configuration details into configuration files, allowing the system to be reconfigured without recompilation.
4.	Separate configurations can be written for different situations that require different implementations of components. This includes, but is not limited to, testing.
5.	Due to decoupling, the reusability of the code is increased.
6.	Improved code maintainability.
7.	It can be applied to legacy code as a code refactoring.
8.	The ease of testing is often the first benefit noticed when using dependency injection.
9.	It allows reduction of boilerplate code in the application objects, since all work to initialize or set up dependencies is handled by a provider component. 
10.	Improves application testing, since stubs can be substituted for any dependency.
	
Even though there are uncountable benefits of using Dependency Injection, it is of utmost importance to check the drawbacks and disadvantages provided by it. From encouraging dependence on a dependency injection framework to forcing complexity to move out of classes and into the linkages between classes, which might not always be desirable or easily managed, there are several disadvantages of dependency injection. 

**Disadvantages of dependency Injection:**
1.	Using many instances together can become a very difficult if there are too many instances and many dependencies that need to be resolved.
2.	Code can become harder to understand.
3.	Dependency injection can make code difficult to trace (read) because it separates behavior from construction. This means developers must refer to more files to follow how a system performs.
</blockqoute> 
</details>

---

8. Why is Dependency Injection Useful?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
	
DI a very useful technique for testing, since it allows dependencies to be mocked or stubbed as required. Every layer (DAO, service, controller) of application can be tested independently.

**Explanation**<br>
Dependency injection plays an important role in test driven development of a software, and it is a design paradigms that is used by software programmers all over the world. Moreover, this framework takes care of creating complicated and advanced objects for developers without allowing them to worry about providing right elements or ingredients. However, the importance of dependency injection is extremely high for unit testing, validation and exception management, as it is tremendously helpful to them in various ways. Hence, elaborated here is the use of dependency injection in unit testing and validation or exception management.<br>
**Unit Testing:** In unit testing, dependency injection enables one to replace complex dependencies, such as databases, with mocked implementations of those dependencies. This further allows them to completely isolate the code that is being tested by the team of expert testers.<br>
**Validation or Exception Management:** With the assistance of dependency injection, an individual can inject additional code between the available dependencies. Also, it is possible to inject exception management logic or validation logic, which means that the developer no longer needs to write similar logic for every phase of development.<br>
</blockqoute> 
</details>

---
