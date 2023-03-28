1.What is use of Netflix Zuul-Duplicated?

![Complex](<https://raw.githubusercontent.com/revaturelabs/interviewquestions/aef8eff919a3b083089641381ed9a9101ed21fba/ComplexityTags/Complex%20(2).svg>)

<details markdown="1"> <summary> <b> Show Answer </b> </summary>

<blockquote markdown="1"> 
    
- Netflix Zuul is an API Gateway server.
- Zuul Server dynamically routes the requests to the respective backend microservice application.
- For Example, all request starting with /api/account are mapped to account service and those starting with /api/sales are mapped to the sales service.
- It works as a front door for all the requests.
- Zuul is built to enable dynamic routing, monitoring, resiliency, and security.
- Zuul is a JVM-based router and server-side load balancer from Netflix.
</blockquote>

</details>

---
