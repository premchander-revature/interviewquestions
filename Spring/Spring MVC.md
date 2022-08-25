## Technical

1. What is DispatcherServlet in Spring MVC application?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- In the case of Spring MVC, DispatcherServlet is the front controller. 
- DispatcherServlet acts as an entry and exit point for any request received from client. 
</blockquote> 

</details>

---

2. How DispatcherServlet handles request & response in Spring MVC application?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- Whenever a request comes it first goes to the DispatcherServlet where it then tries to identify its handler method (the methods defined in the specific controller to handle the requests) using  Handler mapping.
- Once the handler mapping returns the controller the DispatcherServlet knows the controller which can handle the request and goes there for further request processing.
- Once the controller returns view the DispatcherServlet goes to the view resolver to identify where the view is located.
- DispatcherServlet then grabs the view and returns it back as final response.
</blockquote> 

</details>

---

3. How Spring MVC DispatcherServlet is registered in the web.xml file?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- Since DispatcherServlet is one type of Servlet the web.xml file configuration is same as normal servlet.
- Additionally, as DispatcherServlet is our front controller we need to ensure that all the incoming requests should be routed to it using "/" url pattern.
```xml
<servlet>
    <servlet-name>dispatcher</servlet-name>
    <servlet-class>
        org.springframework.web.servlet.DispatcherServlet
    </servlet-class>
</servlet>
<servlet-mapping>
    <servlet-name>dispatcher</servlet-name>
    <url-pattern>/</url-pattern>
</servlet-mapping>
```
- If we are using `spring-boot-starter-web` starter, DispatcherServlet is auto configured to the URL pattern "/". So, we don't need to do any additional configuration in the web.xml file. 
</blockquote> 

</details>

---
4. How to change default context path and url pattern of DispatcherServlet in Spring MVC?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- It's very simple, we need to change two properties inside application.properties file.
```
server.servlet.context-path=/admin
spring.mvc.servlet.path=/v2
```
- With above customizations, DispatcherServlet is configured to handle the URL pattern /v2 and the root contextPath will be /admin. 
- Thus, DispatcherServlet listens at http://localhost:8080/admin/v2/.
</blockquote> 

</details>

---

5. Can we have one `@RestController` class with multiple `@GetMapping` methods?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- Yes, we can have one `@RestController` class with multiple `@GetMapping` methods.
- Defining not only Get but any HTTP method compliant mappings purely depend on the context of application and its use cases.
- Below three GetMappings can be defined inside one UserRestController.
```java
@RestController
public class UserRestController{
    @GetMapping(path="/users/")
    public ResponseEntity<UserInfoDTO> getUserByUsername(@RequestParam String username) {
    }
    // GET user details by username: <protocol>://<hostUrl>/users?username=<username>

    @GetMapping(path="/users")
    public ResponseEntity<List<UserInfoDTO>> getAllUsers() {
    }
    // GET all user details: <protocol>://<hostUrl>/users

    @GetMapping(path="/users/{id}")
    public ResponseEntity<UserInfoDTO> getUserById(@PathVariable Long id)
    // GET user details for specific userid: <protocol>://<hostUrl>/users/<userid>
}
```
</blockquote> 

</details>

---
6. How you ensure both "/" and "/welcome" request mappings land to "index" view in Spring MVC applications?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- `@RequestMapping` annotation in Spring MVC has a String[] value parameter, so we can specify multiple values like below to return index view from controller class as below:
```java
@RequestMapping(value={"/", "welcome"})
public String homePage(){
  return "index";
}
```
</blockquote> 

</details>

---
7. Can @Controller annotation be used for both Spring MVC and RESTful applications?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- Yes, @RestController is a convenience annotation that does nothing more than adding the @Controller and @ResponseBody annotations.
- Hence the following two controller definitions are same:

```java
@Controller
@ResponseBody
public class RestControllerA { 

}

@RestController
public class RestControllerB { 

} 
```
</blockquote> 

</details>

---
8. What does @Controller & @RestController returns?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- @Controller return a view in Spring MVC application.
- @RestController returns an object as response instead of view.
</blockquote> 

</details>

---
9. What is use of @ResponseBody in Spring?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- @ResponseBody is a Spring annotation which binds a method return value to the web response body. 
- It is not interpreted as a view name. 
- It uses `org.springframework.http.converter Interface HttpMessageConverter<T>` to convert the return value to HTTP response body, based on the content-type in the request HTTP header.
</blockquote> 

</details>

---
10. What are MIME Types?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- MIME stands for Multi-purpose Internet Mail Extensions. 
- MIME types form a standard way of classifying file types on the Internet. 
- Internet programs such as Web servers and browsers all have a list of MIME types, so that they can transfer files of the same type in the same way, no matter what operating system they are working in.
- A MIME type has two parts: a `type` and a `subtype`. They are separated by a slash (`/`) i.e., `type/subtype`. 
- For example, the MIME type for Microsoft Word files is application and the subtype is msword. Together, the complete MIME type is application/msword.
- The entire list of MIME types is available under Internet Assigned Numbers Authority (IANA) website- https://www.iana.org/assignments/media-types/media-types.xhtml
- The MIME types & extensions can be found under-https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types/Common_types 
</blockquote> 

</details>

---
11. What is use of `@RequestBody` in Spring?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- `@RequestBody` annotation binds request body to method parameters. 
- We use the `@RequestBody` annotation to have the request body read and deserialized into an Object through an `HttpMessageConverter`. 
- Additionally, automatic validations can be applied by annotating the argument with @Valid annotation.
</blockquote> 

</details>

---
12. What is the meaning of Content Negotiation?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- Content negotiation is the process of selecting one of multiple possible representations to return to a client, based on client or server preferences.
- When a consumer sends a request, it can specify two HTTP Headers related to Content Negotiation `Accept` and `Content-Type`.
- `Content-Type` indicates the content type of the body of the request.
- `Accept` indicates the expected content type of the response.
</blockquote> 

</details>

---
13. What is REST? Is it protocol dependent?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- REST is about resource state manipulation through their representations on the top of stateless communication between client and server. 
- It's a protocol independent architectural style but, in practice, it's commonly implemented on the top of the HTTP protocol.
</blockquote> 

</details>

---
14. What is "representation", "state" and "transfer" in Representational State Transfer (REST)?

![Complex](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Complex%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 

- To understand REST lets first understand-    
  - What is a `resource`- 
    - The key abstraction of information in REST is a resource. 
    - There is no restriction on what a resource can be. 
    - Any information that can be named can be a resource: a document or image, a temporal service (e.g., "today's weather in Los Angeles"), a collection of other resources, a non-virtual object (e.g., a person), and so on.
  - What is a `representation`-
    - A JSON document can be used to represent the state of a particular resource. A resource can have many representations, such as JSON and/or XML documents, and the client can use content negotiation to request different representations of the same resource.
  - What is a `state transfer`-
    - The state of a given resource can be retrieved and manipulated using representations.
</blockquote> 

</details>

---
15. What is REST API versioning? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- API versioning is the process of transparently managing changes to your API.
- Versioning aims at effective communication around changes to API, so consumers/subscribers know what to expect from it. 
</blockquote> 

</details>

---
16. How do we provide version to RESTful APIs in Spring?

![Complex](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Complex%20(2).svg)

<details> <summary> <b> Show Answer </b> </summary>

<blockquote> 
    
- APIs only need to be up-versioned when a breaking change is made. Breaking changes include:
  - Change in the format of the response data for one or more calls
  - Change in the request or response type (i.e., changing an integer to a float)
  - Removing any part of the API.
- There are multiple ways to version RESTful API-
  - One controller class with multiple methods having separate versions for mapping URLs.
  - One controller class with one method having separate versions number passed as path variables.
  - One controller class with one method having separate versions number passed as custom request header.
  - Multiple controller classes marked with version name with their own method names. 
- Breaking changes should always result in a change to the major version number for an API or content response type.
- Non-breaking changes, such as adding new endpoints or new response parameters, do not require a change to the major version number.
- Example of using two controller classes serving to different version-
```java
```
</blockquote> 

</details>

---
