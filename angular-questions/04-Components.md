1. What is a component?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Components are the basic building blocks in the Angular application. Components contain the data & UI logic that defines the view and behavior of the web application.

![image](https://user-images.githubusercontent.com/70228962/186086415-c49cc203-e383-43c0-bc5b-15e2f101f159.png)

Consider, we are building a page for an application. The features in the page include the header, footer and navigation and content area. Instead of building a single page with all these features, we can choose to split the page into components, which help us to manage our application. In the above scenario, we can say that the header, footer, content area, navigation and so on are separate components of the page; but when the user views it on the website through any device, it will show as a single page.
	
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
   
When we run `ng g c server` in the terminal, CLI creates a component and registers this component in the AppModule. Now, you're able to see a `server` folder inside `src/app`. This `server` folder contains 4 files - `server.component.html`, `server.component.spec.ts`, `server.component.ts` and `server.component.css`. 

</blockquote>
</details>
  
---
  
5. Angular Components Lifecycle or Lifecycle Hooks or LifeCycle Methods
  
<details>
<summary> <b>Show Answer</b></summary>
  
<blockquote>
  
Angular creates a component; renders it; creates and renders its children; checks it when it’s data-bound properties change; and destroys it before removing it from the DOM. These events are called "Lifecycle Hooks".

Lifecycle Hooks:	
- `constructor()` - The constructor of the component class gets executed first, before the execution of any other lifecycle hook events. If we need to inject any dependencies into the component, then the constructor is the best place to do so.
- `ngOnChanges()` - Called whenever the input properties of the component change. It returns a SimpleChanges object which holds any current and previous property values.
- `ngOnInit()` - Called once to initialize the component and set the input properties. It initializes the component after Angular first displays the data-bound properties.
- `ngDoCheck()` - Called during all change-detection runs that Angular can't detect on its own. Also called immediately after the `ngOnChanges()` method.
- `ngAfterContentInit()` - Invoked once after Angular performs any content projection into the component’s view.
- `ngAfterContentChecked()` - Invoked after each time Angular checks for content projected into the component. It's called after `ngAfterContentInit()` and every subsequent `ngDoCheck()`
- `ngAfterViewInit()` - Invoked after Angular initializes the component's views and its child views.
- `ngAfterViewChecked()` - Invoked after each time Angular checks for the content projected into the component. It called after `ngAfterViewInit()` and every subsequent `ngAfterContentChecked()`
- `ngOnDestroy()` - Invoked before Angular destroys the directive or component.

</blockquote>  
</details>
	
---  

6. What is use of `@Component` decorator?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
	
<details>
<summary><b>Show Answer</b></summary>
<blockquote>

- Components in Angular are defined using a `@Component` decorator. It includes a selector, template, style, and other properties, and it specifies the metadata required to process the component.

</blockquote>
</details>
  
---

7. How many components can angular have?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Angular applications can have multiple components. Each component handles a small part of UI. These components work together to produce the complete user interface of the application.

</blockquote>
</details>
  
---

8. What is the root component in Angular?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

An Angular application has one root component - `AppComponent`

</blockquote>
</details>
  
---
	
9. How do you find which is a root component?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

By default, the root component in angular is `AppComponent` which is specified in the `bootstrap` array under the `@NgModule` defined in the `app.module.ts` file.

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

10. I have to create component `user` as a parent. Then, I want to 2 child components for `user` component. Let's say 2 child components are `user-login` and `user-register`. What are the steps I needed to do?
	
![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

**Steps:**
1. Run `ng g c user` in the terminal, CLI creates a component and registers this component in the AppModule.  Now, you're able to see a `user` folder inside `src/app`.
2. Move to the `src/app/user` folder.
3. Run `ng g c user-login` in the terminal, CLI creates `user-login` component
4. Run `ng g c user-register` in the terminal, CLI creates `user-register` component

![image](https://user-images.githubusercontent.com/70228962/186089554-ec5c403b-dd95-4f13-83ce-2bd90e4b67c2.png)

</blockquote>
</details>
  
---
	
11. Below is the code in `user.component.ts`. If I want to insert user component to the `index.html` file.
```ts
import { Component } from '@angular/core';
@Component ({
  selector: 'user'
  templateUrl: './user.component.html' ,
  styleUrls: ['./user.component.css']
export class UserComponent {
} 
```
 
![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Using `<user>` tag in the `index.html`

</blockquote>
</details>
  
---
	
12. Detail about `@Component` Decorator.
	
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)	

<details>
<summary> <b>Show Answer</b></summary>
<blockquote>

In `app.component.ts` file, we export the `AppComponent` class, and we decorate it with the `@Component` decorator, imported from the `@angular/core package`, which takes a few metadata, such as: `selector`, `templateUrl` and `styleUrls`.

```ts
import { Component } from '@angular/core';

@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
export class AppComponent {
  title = 'angularDemoProject';
}
```
- `selector` – just name given for the component. In the `index.html` file, `<app-root>` tag corresponds to component’s selector. By doing so, Angular will inject the corresponding template of the component. 
```html
<body>
  <app-root></app-root>
</body>
```
- `templateUrl` - points to an HTML file that defines what you see on your application. 
- `styleUrls` - points to set of CSS file that defines styles or design for application

</blockquote>
</details>
	
---   

13. What is a template in Angular?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

A template just like regular HTML that renders a view, or user interface, in the browser.

When you generate an Angular application with the Angular CLI, the `app.component.html` file is the default template containing placeholder HTML.

</blockquote>
</details>
  
---
 
 14. What is the difference between `templateUrl` and `template` in `@Component` decorator?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>


</blockquote>
</details>
  
---
 	
	
15. What is the difference between `styleUrls` and `styles` in `@Component` decorator?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
 
16. Which lifecycle hook will be executed first?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
 
17. Which lifecycle hook used to inject any dependencies into the component?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
 
18. In which order does lifecycle hooks gets exceuted?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
 
19. Which lifecycle called only one?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
 
20. Which angular module has all lifecycle hooks interfaces?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
	
21. Can we have html content attached to the component without having `.html` file. If so, how?
	
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
	
22. Can we have css styles attached to the component without having `.css` file. If so, how?
	
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
	
23.  Can we have multiline template? If so, how?
	
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
	
24. What is a views in Angular?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
	
25. How view is different from template?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---

26. What are ways to define templates?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

There are two ways of defining template in an angular component.
1. Inline Template
2. Template file
	
Inline Template  - It is defined by placing the HTML code in back ticks _`_ and is linked to the component metadata using the `template` property of `@Component` decorator.
```ts
@Component({
  selector: 'app-root',
  templateUrl: `<h1> Hello World </h1>`,
  styleUrls: ['./app.component.css']
})
````
Template File - It is defined in a separate HTML file and is linked to the component metadata using the `@Component` decorator’s `templateUrl` property 
	
```ts
@Component({
  selector: 'app-root',
  templateUrl: './app.component.html',
  styleUrls: ['./app.component.css']
})
```

</blockquote>
</details>
  
---
 
