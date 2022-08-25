1. What are Pipes in angular? Explain with example. 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Pipes provide a way to transform values in an Angular template. Pipes are used with a Pipe (`|`) character, and take integers, strings, arrays, and date as input and returns a desired formatted output which can be displayed in the browser.
    
For example, a Date object shows the date in this format: `Sat Aug 03 2019 19:48:11 GMT+0530 (India Standard Time)` which is not easy for the normal users to understand. It’s better to have the date in this format `Saturday, 03 Aug 2019 07:50 PM`. This can be achieved using pipes.

</blockquote>
</details>
  
---
 
2. How you can transform any strings, currency amounts, dates, and other data for display?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

Using Pipes 

</blockquote>
</details>
  
---
 
3. What happens if I decorate class with `@Pipe` decorator?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

If we want to create a custom pipe in angular, we need to annotate the class with `@Pipe` decorator.

`@Pipe` decorator has a name property, which used to specify the name of the pipe. 
  
</blockquote>
</details>
  
---
 
4. Detail the use of below code:
```ts
interface PipeTransform {
  transform(value: any, ...args: any[]): any
}
```
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>

An interface that is implemented by pipes in order to perform a transformation. Angular invokes the `transform` method with the value of a binding as the first argument, and any parameters as the second argument in list form.

</blockquote>
</details>
  
---
 

5. Can we create our own pipe in angular? If so, how?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)


<details>
<summary><b>Show Answer</b></summary>
<blockquote>
  
 Yes, we can our own pipe in angular. 
  
**For example:** we create a custom pipe to get first character in a given string, by running the `ng g pipe firstChar` command in the terminal. The CLI creates 2 files - `first-char.pipe.spec.ts` and `first-char.pipe.ts` under _src/app_ folder and updates the `app.module.ts` file.

In `first-char.pipe.ts` file, we write the logic for returning first character in a given string.
  
```ts
import { Pipe, PipeTransform } from '@angular/core';
@Pipe({   name: 'firstChar' })
export class FirstCharPipe implements PipeTransform {

  transform(value: string): string{
    return value[0];
  }
}  
```
And, we can use it any template file. For example,  in `app.component.ts` file,
  
```ts
{{ "Hello World" | firstChar}}  
```
  
</blockquote>
</details>
  
---
 
6. Design the angular application to print current date in this format "MM/dd/yy".

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
 
7. Design the angular application to get a sentence form user and print the count of words in the given sentence.

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
 
8. Design the angular application to print the list of groceries items followed by its price in rupees

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
 
9. How can slice the strings?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
 
10. List some of the built in pipes in angular. 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---

11. Design the angular application to print user's brithday in this format "MAY 19, 1997".
 
![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---

12. What is use of `PipeTransform` in angular?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b>Show Answer</b></summary>
<blockquote>



</blockquote>
</details>
  
---
