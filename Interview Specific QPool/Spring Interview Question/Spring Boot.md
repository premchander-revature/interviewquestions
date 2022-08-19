## Spring Boot

1. What is Spring Boot?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>

Spring Boot is basically an extension of the Spring framework, it allows us to build a stand-alone application based on the jar dependencies you have enabled, with less or nearly zero configuration. 

**Explanation**<br> It takes an opinionated ‘starter' dependencies to simplify the build and application configuration, which paves the way for a faster and more efficient development ecosystem. Mostly with Spring Boot, we just need to notify Spring how many plugins we want to use, and we’ll get a quick setup for them. We can use the spring initializer to pull our application into all the dependencies we need, thereby reducing our development time. Spring Boot assists in faster development as it has a lot of starter projects that help you get moving very quickly. Many non-functional features are also included, such as embedded servers, some metrics, health checks, safety, etc. In short, with minimal invasion of code, it makes Spring-based application creation simpler. It comes with the starter definition in the pom.xml file that takes care of installing the JAR dependencies depending on the Spring Boot Requirement. All in all, Spring Boot is a project initializer based on Spring. It prevents you from writing long code with features such as auto-configuration and lets you avoid excessive configuration.
</blockqoute> 
</details>

---

2. When should you use Spring Boot vs. Spring?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
  
It is better to use Spring Boot if we want to develop a simple Spring-based application or RESTful services.
</blockqoute> 
</details>

---

3. What is difference between Spring Boot vs. Spring?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>

|     Spring   Boot                                                                                                                                                          |     Spring                                                                                       |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
|     Autoconfiguration is the primary feature of Spring   Boot                                                                                                              |     Dependency Injection is the primary feature of   Spring                                      |
|     Spring Boot Framework is widely used to develop REST   APIs.                                                                                                           |     Spring Framework is a widely used for building Java   SE, Java EE applications.              |
|     It aims to shorten the code length and   provide the easiest way to develop Web Applications.                                                                          |     It aims to simplify Java EE development that makes   developers more productive.             |
|     The primary feature of Spring Boot is   Autoconfiguration. It automatically configures the classes based on the   requirement.                                         |     The primary feature of the Spring Framework is dependency   injection.                       |
|     It helps to create a stand-alone application with   less configuration.                                                                                                |     It helps to make things simpler by allowing us to   develop loosely coupled applications.    |
|     It reduces boilerplate code.                                                                                                                                           |     For smaller tasks, developers need to write a   boilerplate code                             |
|     Spring Boot offers embedded server such as Jetty and   Tomcat, etc.                                                                                                    |     To test the Spring MVC project, we need to set up   the sever explicitly.                    |
|     Spring Boot comes with the concept of starter in   pom.xml file that internally takes care of downloading the dependencies JARs   based on Spring Boot Requirement.    |     Developers manually define dependencies for the   Spring project in pom.xml.                 |
|     There is no requirement for a deployment descriptor i.e.,   web.xml file.                                                                                              |     For Spring MVC applications a deployment descriptor   is required.                           |
  
  ![image](https://user-images.githubusercontent.com/99252558/185605265-237355ae-7024-43ca-8ee6-6817570c79fd.png)
