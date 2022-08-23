1. What is a component?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Components are the basic building blocks in the Angular application. Components contain the data & UI logic that defines the view and behavior of the web application.

</blockquote>
</details>
  
---

2. In which file, I can find `@Component` decorator?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
  
 `app.component.ts` 
  
</blockquote>
</details>
  
---

3. How do you create a component?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>
  
 Run the `ng generate component <component_name>` or `ng g c <component-name>` command in the terminal to create a component

</blockquote>
</details>
  
---
  
 4. What are the files created or updated when we create a component?
 
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
  
<details>
<summary><b>Show Answer</b></summary>
<blockquote>
   
When we run `ng g c server` in the terminal, CLI creates a component and registers this component in the AppModule. Now, you're able to see a *server* folder inside *src/app*. This *server* folder contains 4 files - *server.component.html*, *server.component.spec.ts*, *server.component.ts* and *server.component.css*. 

</blockquote>
</details>
  
---
  
5. Angular Components Lifecycle or Lifecycle Hooks or LifeCycle Methods
  
<details>
<summary> <b>Show Answer</b></summary>
  
<blockquote>
  
- Angular creates a component; renders it; creates and renders its children; checks it when it’s data-bound properties change; and destroys it before removing it from the DOM. These events are called "Lifecycle Hooks".
- Lifecycle Hooks:
	
  ![image](https://user-images.githubusercontent.com/103101208/185570891-363fb6d0-3bcd-454e-b2da-68362092fe64.png)
	
- `constructor()` - The constructor of the component class gets executed first, before the execution of any other lifecycle hook events. If we need to inject any dependencies into the component, then the constructor is the best place to do so.
- `ngOnChanges()` - Called whenever the input properties of the component change. It returns a SimpleChanges object which holds any current and previous property values.
- `ngOnInit()` - Called once to initialize the component and set the input properties. It initializes the component after Angular first displays the data-bound properties.
- `ngDoCheck()` - Called during all change-detection runs that Angular can't detect on its own. Also called immediately after the ngOnChanges() method.
- `ngAfterContentInit()` - Invoked once after Angular performs any content projection into the component’s view.
- `ngAfterContentChecked()` - Invoked after each time Angular checks for content projected into the component. It's called after `ngAfterContentInit()` and every subsequent `ngDoCheck()`
- `ngAfterViewInit()` - Invoked after Angular initializes the component's views and its child views.
- `ngAfterViewChecked()` - Invoked after each time Angular checks for the content projected into the component. It called after `ngAfterViewInit()` and every subsequent `ngAfterContentChecked()`
- `ngOnDestroy()` - Invoked before Angular destroys the directive or component.
	
![image](https://user-images.githubusercontent.com/103101208/185571059-270e2558-e7f9-48e9-8023-3cb594a8d780.png)

</blockquote>  
</details>
	
---  
