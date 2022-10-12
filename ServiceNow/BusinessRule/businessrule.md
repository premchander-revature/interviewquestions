1. What is the use of notifications in servicenow? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
The business rule is a server-side script that launches whenever a table is queried, or whenever a record is displayed, inserted, updted or deleted.

</blockquote>
  
</details>

---

2. What are the types of business rule? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
Business rules can be divided into four categories: before, after, async, and display.

</blockquote>
  
</details>

---

3. When does the before business rule trigger?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
Before business rule is triggered when a user submits the form, but before any action is taken on the record in the database.

</blockquote>
  
</details>

---

4. When does after business rule triggers?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
When a user submits the form and any action is taken on the database record, then the after business rule is triggered.

</blockquote>
  
</details>

---

5. What is the use of setworkflow() in servicenow?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
The serWorkflow() method accepts one argument: a boolean true/false value. This argument will determine whether business rules should be triggered by any database actions performed by your GlideRecord script. For example, if you make a change and call the update() method, calling setWorkflow() and passing in false will prevent any business rules that would normally be triggered by that update from running.

</blockquote>
  
</details>

---