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


</blockqoute> 
</details>

---

4. What are some of the annotations you've used in Spring Boot?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
    
 Spring Annotations are a form of metadata that provides data about a program. Annotations are used to provide supplemental information about a program. Spring annotations present in the `org.springframework.boot.autoconfigure` and `org.springframework.boot.autoconfigure.condition` packages are commonly known as Spring Boot annotations. Some of the annotations that are available in this category are as follows: 
1.	**@SpringBootApplication** - This annotation is used to mark the main class of a Spring Boot application. It encapsulates @SpringBootConfiguration, @EnableAutoConfiguration, and @ComponentScan annotations with their default attributes.
2.	**@ComponentScan** - It is used when we want to scan a package for beans. Generally, @ComponentScan annotation is used with @Configuration annotation to specify the package for Spring to scan for components. We can also specify the base packages to scan for Spring Components. It tells Spring in which packages you have annotated classes that should be managed by Spring. For example, if you have a class annotated with @Controller which is in a package that is not scanned by Spring, you will not be able to use it as a Spring controller. So, we can say @ComponentScan enables Spring to scan for things like configurations, controllers, services, and other components that are defined. 
3.	**@EnableAutoConfiguration** - It auto-configures the bean that is present in the class path and configures it to run the methods. The use of this annotation is reduced in Spring Boot 1.2.0 release because developers provided an alternative of the annotation, i.e., @SpringBootApplication. For example, when we illustrate the spring-boot-starter-web dependency in the class path, Spring boot auto-configures Tomcat, and Spring MVC. The package of the class declaring the @EnableAutoConfiguration annotation is considered as the default. Therefore, we need to apply the @EnableAutoConfiguration annotation in the root package so that every sub-packages and class can be examined.
4.	**@Configuration** - It is a class-level annotation. The class annotated with @Configuration used by Spring Containers as a source of bean definitions.
5.	**@SpringBootConfiguration** - It can be used as an alternative to Spring’s standard @Configuration annotation so that configuration can be found automatically. Most Spring Boot Applications use @SpringBootConfiguration via @SpringBootApplication.
</blockqoute> 
</details>

---

5. How to create Spring Boot project? Or What is Spring Initializr? How would I go about writing a spring boot application to expose endpoints?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
    
 The easiest way to build Spring Boot project is to used Spring Initializr module. Spring Initializr provides an extensible API to generate JVM-based projects, and to inspect the metadata used to generate projects, for instance to list the available dependencies and versions. 
    
**Explanation**<br> With Spring Initializr, there is minimal code involved and the service has a very rich configuration structure, allowing you to define not only the values of various project attributes but also the list of dependencies and the constraints to apply to them. The API can be used standalone or embedded in other tools (e.g., it is used in major IDEs such as Spring Tool Suite, IntelliJ IDEA Ultimate, NetBeans and VSCode).

Steps:<br>
1.	Navigate to `https://start.spring.io.` This service pulls in all the dependencies you need for an application and does most of the setup for you.
2.	Choose either Gradle or **Maven** and the language you want to use. This guide assumes that you chose Java.
3.	Click **Dependencies** and select **Spring Web**, **Spring Data JPA**, and **MySQL** Driver.
4.	Click **Generate**.
5.	Download the resulting ZIP file, which is an archive of a web application that is configured with your choices.
6.	Open the project into any java IDE.
7.	Configure standard package names.
8.	Define various configuration details for your spring application e.g., DB server details under each `application-<spring-profile-name-by-region>.properties` file.
9.	Configure various entities used in project using respective ORM provider.
10.	Implement DAO layer repositories using either **JpaRepository** or **CrudRepository** (We prefer using **JpaRepository** due to its additional benefits) and using `@Repository` annotation.
11.	Implement service layers using more business specific functionalities by injection one or more repositories.
12.	Implement controller layer using `@Controller` or `@RestController`  depending upon business requirements.
13.	Expose various endpoint methods using appropriate request mapping annotations like. `@GetMapping`, `@PostMapping`, `@PutMapping`  or `@DeleteMapping`
14.	Test Application using any client like SoapUI, Postman etc.

</blockqoute> 
</details>
    
 ---
    
 6. What are the standard package names which are followed by any enterprise java application?
 
![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>

Usually there is no restriction on whatever the package name you provide for your application, but as per industry standards and enterprise application being divided into various layered structure the standard package structures which can be defined in project are listed below 
    
1.	`com.revature.model`  - This will have all your POJOs and JPA entities defined.
2.	`com.revature.repositories` or `com.revature.dao`  - This will have all you @Repositries or any DAO interface & classes defined.
3.	`com.revature.service` - This will have all you @Service interface & classes defined.
4.	`com.revature.controller` - This will have all you @Controller or @RestControllers classes defined.
5.	`com.revature.constants` - This will have all your classes with private constructor and all public static final constants defined.
6.	`com.revature.util` - This will have all your own utility classes defined e.g.pdf, csv export file utilities, encryption/decryption.
7.	`com.revature.config` - This will have all your spring @Configuration classes with @Bean definitions.
8.	`com.revature.dto`  - This will have all your Data Transfer Object (DTO) classes defined which are usually subsets of attributes from different POJO and Entity classes.
9.	`com.revature.test.unit` - This will have all your application jUnit test cases defined.
10.	`com.revature.test.api` - This will have all your application integration test cases defined.
</blockqoute> 
</details>
    
---

7. What is the standard Spring profile per region properties file names followed by any enterprise java application?
    
![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
    
Usually there is no restriction on whatever the profile names you use but as per industry standards you can use below spring profile and respective properties file name-
1.	`application.properties`  - Spring Default profile
2.	`application-dev.properties`  - Spring Dev Profile for Development Region
3.	`application-int.properties`  - Spring Dev Profile for Integration Testing Region
4.	`application-uat.properties`  - Spring Dev Profile for User Acceptance Testing Region
5.	`application-staging.properties`  - Spring Dev Profile for User Staging/Performance Testing Region
6.	`application-preprod.properties`  - Spring Dev Profile for Pre-Production or Sandbox Region
7.	`application-prod.properties`  - Spring Dev Profile for PROD Region
</blockqoute> 
</details>
    
---
    
8. Which IDE can be used to build Spring Boot application?
    
![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
    
You can use any latest version of Eclipse, Spring Tool Suite, IntelliJ Idea, Visual Studio Code or any other IDE compliant with your enterprise guidelines. Out of all the IDE spring recommended to use Spring Tool Suite since it has Spring Initializr integration integrations preconfigured for other IDEs you may need to configure Spring plugins manually.
</blockqoute> 
</details>
    
---

9. How does Spring Boot Application Bootstraps?
    
 ![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>

 The entry point of execution of a Spring Boot application is the class that is annotated with `@SpringBootApplication`. 
    
``` java
@SpringBootApplication
public class Application {
    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }
}
```
    
Spring boot application uses embedded container to run the application. Spring Boot uses the public static void main entry point to launch an embedded web server. The binding of the Servlet, Filter, and ServletContextInitializer beans from the application context to the embedded servlet container is take care internally. It automatically scans all the classes in the same package or sub packages of the Main-class for components. In addition, Spring Boot provides the option of deploying it as a web archive in an external container for this we have to extend the SpringBootServletInitializer as follows, Here the external servlet container looks for the Main-class defined in the META-INF file of the web archive, and the SpringBootServletInitializer will take care of binding the Servlet, Filter, and ServletContextInitializer.
    
 ``` java
 @SpringBootApplication
public class Application extends SpringBootServletInitializer {
    // ...
}
```
    
---
