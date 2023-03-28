1.Consider you have a list which holds values of multiple datatypes how do you extract only the numbers from that list?

![Medium](<https://raw.githubusercontent.com/revaturelabs/interviewquestions/aef8eff919a3b083089641381ed9a9101ed21fba/ComplexityTags/Medium%20(2).svg>)

<details markdown="1"><summary><b>Show Answer </b></summary>
<blockquote markdown="1">
  
- In a list, Python can contain different types of data, and an item in the list is separated by a comma and the entire list is enclosed in square brackets [].
- If we want to Extract only the numbers from the list, we can use `isinstance()` method through the loop `isinstance(int,float)`.Checking list contains numbers.If not, it contains int and float and it will store in another list, and we will print the list.

**Example**:

```python
list1 = ["a", 1, "b", 2, 3, 4, "c", "d"]
list2 = [val for val in list1 if isinstance(val, (int, float)]
print(list2)
```

**Output:**

[1, 2, 3, 4]

</blockquote>

</details>
  
---
