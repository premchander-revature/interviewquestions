1. What is Eager and Lazy loading?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
  
**Eager Loading:** 
- It is the default module-loading strategy. 
- It loads the feature modules are loaded before the program begins. 
- This is primarily utilized for small-scale applications.

**Lazy Loading:** 
- It loads the feature modules dynamically as needed. 
- This speeds up the application. 
- It is utilized for larger projects where all of the modules are not required at the start.

</blockquote>
</details>
  
---

2. Does Angular lazy loads the modules?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
 
No. By default, Angular loads the NgModules eagerly which means that as soon as the application loads, all the NgModules & components loaded, whether or not they are immediately necessary.

</blockquote>
</details>
  
---

3. Which do you thinks its best eagerly loaded or lazy loaded?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
 
For small scale application, eagerly loading modules would be good. But as the application grows the load time will increase if everything is loaded at once. Lazy loading allows Angular to load components and modules as and when they're needed.
  
For large scale application, lazy loading modules would be good.
  
</blockquote>
</details>
  
---

4. What are NgModules?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
  
- NgModules consist of files and code related to a specific domain or that have a similar set of functionalities.
- A typical NgModule file declares components, directives, pipes, and services. 
- It can also import other modules that are needed in the current module.
- Angular libraries like `RouterModule`, `BrowserModule`, `HttpClientModule` and `FormsModule` are NgModules. 
- One of the important advantages of NgModules is that **they can be lazy loaded**.
  
</blockquote>
</details>
  
---

5. List benefits of lazy loading.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
 
Benefits of lazy loading module:
- **Reduces initial load time** – Lazy loading a webpage reduces page weight, allowing for a quicker page load time.
- **Bandwidth conservation** – Lazy loading conserves bandwidth by delivering content to users only if it’s requested.
- **System resource conservation** – Lazy loading conserves both server and client resources, because only some of the images, JavaScript and other code actually needs to be rendered or executed.
   
</blockquote>
</details>
  
---

6. Explain the use of `@NgModule` Decorator

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Show Answer</b></summary>
<blockquote>

`@NgModule` takes the below metadata to launch the application:
- `declarations` — contains a list of components, directives, and pipes, which belong to this module.
- `imports` — contains a list of modules, which are used by the component templates in this module reference.  For example, we import `BrowserModule` to have browser-specific services such as DOM rendering, sanitization, and location.
- `providers` — the list of service providers that the application needs.
- `bootstrap` — contains the root component of the application

```ts
import { NgModule } from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { AppComponent } from './app.component';
@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [ 
    BrowserModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```
	
</blockquote>
</details>
	
--- 

7. What is the root module of angular?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary> <b>Show Answer</b></summary>
<blockquote>

`AppModule` - file is `app.module.ts`
	
</blockquote>
</details>
	
--- 
