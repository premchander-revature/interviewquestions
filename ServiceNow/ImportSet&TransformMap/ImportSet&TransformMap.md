1. How can we load data from different data sources in servicenow?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
We can use the import set tool to import the data from different data sources and then, via the use of transform maps, map that data into ServiceNow tables.

</blockquote>
  
</details>

---

2. What is a transform map in ServiceNow?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
A transform map determines the relationships between fields displaying in an import set table and fields in an existing ServiceNow table, such as the Incidents or Users table.

</blockquote>
  
</details>

---

3. Can you explain the foreign record insert with an example?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
When an import makes any modification to the table that is not the target table for that particular import, then a foreign record insert happens. As an example, if you are loading data into an incident table and in the caller field you enter a user who is not present in your user table, then after you import the data, ServiceNow will create a new user if you set the choice action as create. In this scenario, the import of incident records made a change in the user table, which is not the target table for that import.

</blockquote>
  
</details>

---

4. What is meant by Coalesce in ServiceNow?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
Coalesce is a property of a field that we use in transform map field mapping. The field for which we have set the coalesce true will act as a unique key. If any field from the existing records is matched with the coalesce field, then that record is updated; if no field from the existing records is matched with the coalesce field, then a new record is created.

</blockquote>
  
</details>

---

5. How can we reduce the processing time of a transform map if we are importing a large amount of data?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
If we are importing the large amount of data then to reduce the processing time we can split the incoming data into multiple import sets and we can transform the import sets concurrently. 

</blockquote>
  
</details>

---

6. If we have not set coalesce for any of the fields, what impact will it have on the imported records?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
If no coalesce is defined, all the imported rows will be treated as new records. This may result in duplicate records in the target table.

</blockquote>
  
</details>

---

7. What are the file formats supported by the servicenow to import the data?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>

ServiceNow supports CSV, Excel, XML, and JSON file formats.

</blockquote>
  
</details>

---

8. What are the different types of transform map script? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>

There are a total of 3 types of transform map scripts. Explicit, Field Map Script, and Trasformation Event Script.

</blockquote>
  
</details>

---

9. What are the different types of transform event scripts? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>

In the transform event script we have 6 types. onStart, onComplete, onBefore, onForeignInsert, onChoiceCreate, and onReject.

</blockquote>
  
</details>

---

10. How will you set the title field of a user record created by foreing record insert?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>

By using the onForeignInsert type in the transform event script, we can trigger an event and pass the source object with a user name to that event. Then we can link a script action to that event. So whenever the event is triggered, the script action will execute and, by fetching the parameters from the event, we can identify the record and set its field values.

</blockquote>
  
</details>

---

11. When onStart event script is executed? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>

The onStart event script is processed at the start of an import run, before any data rows are read.

</blockquote>
  
</details>

---

12. When onBefore event script is executed? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>

The onBefore event script is processed at the start of a row transformation, before the source row is transformed into the target row.

</blockquote>
  
</details>

---

13. When onChoiceCreate event script is executed? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>

The onChoiceCreate event script is processed at the start of a choice value creation, before the new choice value is created.

</blockquote>
  
</details>

---

14. When onReject event script is executed? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>

The onReject event script is processed during the occurrence of a foreign record or choice creation, and the foreign record or choice is rejected ,the entire transformation row is not saved.

</blockquote>
  
</details>

---