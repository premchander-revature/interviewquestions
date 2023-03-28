1.How SessionFactory gets the hibernate metadata-dup?

![Easy](<https://raw.githubusercontent.com/revaturelabs/interviewquestions/aef8eff919a3b083089641381ed9a9101ed21fba/ComplexityTags/simple%20(2).svg>)

<details markdown="1">
<summary> <b>Show Answer</b> </summary>

<blockquote markdown="1">

```java
SessionFactory sf=new Configuration().configure(“revature.cfg.xml”).buildSessionFactory().
```

</blockquote>

</details>

---
