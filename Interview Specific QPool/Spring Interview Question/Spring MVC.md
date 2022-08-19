## Spring MVC

1. Describe the architecture of Spring MVC

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
<details>
    <summary><b> Show Answer </b></summary> 
<blockquote>
  
Spring MVC is the web component of Spring’s framework which provides a rich functionality for building robust Web Applications. The Spring MVC Framework is architected and designed in such a way that every piece of logic and functionality is highly configurable. It can integrate effortlessly with other popular Web Frameworks like Struts, WebWork, Java Server Faces etc. Spring is not tightly coupled with Servlets or JSP to render the View to the Clients it can be integrated with other view technologies like Velocity, Freemarker etc.
  
**Explanation**<br> Spring MVC, as many other web frameworks, is designed around the front controller pattern where a central **Servlet**, the **DispatcherServlet**, provides a shared algorithm for request processing, while actual work is performed by configurable delegate components. The **DispatcherServlet**, as any Servlet, needs to be declared and mapped according to the Servlet specification by using Java configuration or in web.xml. In turn, the **DispatcherServlet** uses Spring configuration to discover the delegate components it needs for request mapping, view resolution, exception handling, and more.
![image](https://user-images.githubusercontent.com/99252558/185601373-5f78c15d-428c-41ea-882c-cec6fd370072.png)
The request processing workflow in Spring Web MVC (high level):
- The **DispatcherServlet**, as any **Servlet**, needs to be declared and mapped according to the Servlet specification by using Java configuration or in **web.xml**. In turn, the **DispatcherServlet** uses Spring configuration to discover the delegate components it needs for request mapping, view resolution, exception handling etc.
``` xml
<web-app>
    <servlet>
        <servlet-name>app</servlet-name>
        <servlet-class>org.springframework.web.servlet.DispatcherServlet</servlet-class>
        <load-on-startup>1</load-on-startup>
    </servlet>
    <servlet-mapping>
        <servlet-name>app</servlet-name>
        <url-pattern>/app/*</url-pattern>
    </servlet-mapping>
</web-app>
```

- **DispatcherServlet** expects a **WebApplicationContext** (an extension of a plain **ApplicationContext**) for its own configuration. **WebApplicationContext** has a link to the **ServletContext** and the **Servlet** with which it is associated.
- The **DispatcherServlet** delegates to special beans to process requests and render the appropriate responses. By “special beans” we mean Spring-managed Object instances that implement framework contracts. Few special beans detected by the DispatcherServlet are:
    - **HandlerMapping** - Map a request to a defined specific handler (e.g. @RequestMapping annotated methods).
    - **ViewResolver** - Resolve logical String-based view names returned from a handler to an actual View with which to render to the response. Configuring view resolution is as simple as adding viewResolver beans to your Spring configuration. The Spring Framework has a built-in integration for using Spring MVC with JSP and JSTL. When developing with JSPs, you typically declare an **InternalResourceViewResolver** bean.**InternalResourceViewResolver** can be used for dispatching to any Servlet resource but in particular for JSPs. As a best practice, Spring  strongly encourages placing all your JSP files in a directory under the `WEB-INF` directory so there can be no direct access by clients.

``` xml
<bean id="viewResolver" class="org.springframework.web.servlet.view.InternalResourceViewResolver">
    <property name="viewClass" value="org.springframework.web.servlet.view.JstlView"/>
    <property name="prefix" value="/WEB-INF/jsp/"/>
    <property name="suffix" value=".jsp"/>
</bean>
```

---
