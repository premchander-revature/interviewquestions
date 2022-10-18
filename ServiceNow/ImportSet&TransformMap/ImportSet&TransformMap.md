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

