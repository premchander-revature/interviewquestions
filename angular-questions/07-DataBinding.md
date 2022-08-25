1. Consider there is a variable `name = "Angular"` in `app.component.ts, how can I print this value in template.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Using String Interpolation, we can print the `name` in template. In `app.component.html`, 
```html
{{ name }}
```

</blockquote>
</details>
  
---
 
2. Design the angular app with the following criteria
	- Template should have button named `Click Me`
	- When user clicked on the button, you should greet the user with a message "Welcome to my angular app"

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

In `app.component.html`, create a button and have `Click Me` enclosed with `<button>` tag. When user clicked on the button, we should greet the user with a message "Welcome to my angular app". We need data binding. 
	
```html
<button (click)="onClick()"> Click Me</button>	
```

</blockquote>
</details>
	
--- 
	
3. What are the ways of databinding in angular?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
	
<details>
<summary> <b>Show Answer</b></summary>
<blockquote>

- Databinding is a technique used to bind the data from an view to a component or from a component to view.
- They are 1 way databinding and 2-way databinding

![image](https://user-images.githubusercontent.com/70228962/186707770-894831c5-ca53-455e-9a22-553f426c3335.png)

</blockquote>
</details>
	
--- 

4. What is Property Binding? How do you achieve it in Angular?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
	
<details>
<summary> <b>Show Answer</b></summary>
<blockquote>
	
- From Component to the view
- Bind values to the attributes of HTML elements.
- Uses [], square brackets in the html file
- Create a variable in the class, and the bind that value to an attribute for HTML tag

![image](https://user-images.githubusercontent.com/103101208/185592858-66cc92f3-feca-436e-87cf-766c692a8a8c.png)

</blockquote>
</details>
	
--- 

5. How do you achieve event binding in Angular?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
	
<details>
<summary> <b>Show Answer</b></summary>
<blockquote>

- From view to component
- Bind DOM events such as keystrokes, button clicks, mouse overs, touches, etc. to a function in the component.
- Uses (), parentheses in the html file
- Here, we were calling the `OnClick()` function, when the ‘Click Here’ button is clicked.

![image](https://user-images.githubusercontent.com/103101208/185593164-aa23c1a2-497c-4906-8b32-15af3231d0a6.png)

</blockquote>
</details>
	
--- 

6. What is meant by String Interpolation?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
	
<details>
<summary> <b>Show Answer</b></summary>
<blockquote>

- From the component class to the HTML template
- Uses {{}}, double curly braces in the html

![image](https://user-images.githubusercontent.com/103101208/185593247-f546704d-d3ed-4a80-8ff3-01289401fe00.png)

</blockquote>
</details>
	
--- 


7. Do you know about two way databinding in angular? If so, explain.
	
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)
	
<details>
<summary> <b>Show Answer</b></summary>
<blockquote>

- Two-way data binding is achieved by combining property binding and event binding together.
- Mostly used in forms.
- The Angular uses the `ngModel` directive to achieve two-way binding on HTML `<form>` elements.
- To use the `ngModel` directive, we need to import the `FormsModule` package into our Angular module.
- Here, we enclose `ngModel` directive within [()]

![image](https://user-images.githubusercontent.com/103101208/185593434-3e70965a-c750-4bbd-aa3b-b3fea6fccba7.png)

</blockquote>
</details>
	
--- 

8. How we can pass the data from component to the template?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
 


