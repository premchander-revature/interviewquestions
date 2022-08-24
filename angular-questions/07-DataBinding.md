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
