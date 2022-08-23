1. Debug the error in the given below table:
  | Stu_Id |	Stu_Name      |  Stu_Marks    |   Stu_Age  |
  |--------|----------------|---------------|------------|
  |  101   |     Ramesh	    |       92	    |      20    |
  |  100   |     Divya	    |       83	    |      19    |
  |  202   |      Anu	      |       85      |	     19    |
  |  203   |     Monika	    |       95	    |      21    |
  |  102   |     Sanjana    |       65	    |      21    |

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
<summary><b> Show Answer </b></summary>

<blockquote>

```sql

UPDATE Product SET stu_Marks = 80 WHERE Stu_Id = 102 ;

```

  | Stu_Id |	Stu_Name    |  Stu_Marks    |   Stu_Age  |
  |--------|--------------|---------------|------------|
  |  101   |     Ramesh	  |       92	    |      20    |
  |  100   |     Divya	  |       83	    |      19    |
  |  202   |      Anu	    |       85      |	     19    |
  |  203   |     Monika	  |       95	    |      21    |
  |  102   |     Sanjana  |       80	    |      21    |

  <details>
<summary><b>  Explanation  </b></summary>

<blockquote>
 
        To Update a particular row by using update command and the syntax for updating a particular row is ,
         
      `UPDATE` Table_Name  `SET` Column_Name  `WHERE` Condition;
</blockquote>

</details>
</details>