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
 
No. By defeault, Angular loads the NgModules eagerly which means that as soon as the application loads, all the NgModules & components loaded, whether or not they are immediately necessary.

</blockquote>
</details>
  
---
 
