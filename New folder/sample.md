1.What are Zuul Filter & its types-Duplicated?

![Complex](<https://raw.githubusercontent.com/revaturelabs/interviewquestions/aef8eff919a3b083089641381ed9a9101ed21fba/ComplexityTags/Complex%20(2).svg>)

<details markdown="1"> <summary> <b> Show Answer </b> </summary>

<blockquote markdown="1"> 
    
- Netflix Zuul mainly comprises of four types of filters.
- Filter enable us to intercept the traffic in different timeline of the request processing.
- We can add any number of filters for a particular url pattern.
  - `Pre filters` – Invoked before the request is routed.
  - `Post filters` – Invoked after the request has been routed.
  - `Route filters` – Used to route the request.
  - `Error filters` – Invoked when an error occurs while handling the request.
	
</blockquote>

</details>

---
