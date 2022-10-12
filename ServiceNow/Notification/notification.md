1. What is the use of notifications in servicenow? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
Users can be updated about the events that matters to them using notifications in servcienow.

</blockquote>
  
</details>

---

2. What are types of ServiceNow notifications? 

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
Servicenow supports Emails, SMS, and Push Notifications.

</blockquote>
  
</details>

---

3. Where can we configure settings for inbound and outbound email?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
On the Email Properties page, we can configure settings for inbound and outbound email.

</blockquote>
  
</details>

---

4. Which servers are used to send and receive emails in servicenow?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
Servicnow uses an SMTP server to send emails and a POP3 server to receive emails.

</blockquote>
  
</details>

---

5. Is there a size restriction on emails sent or received through ServiceNow?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
For inbound (POP3) and outbound (SMTP) emails, the ServiceNow servers set a maximum total encoded email size of 75 MB and 25 MB, respectively. Emails larger than this are not accepted.

</blockquote>
  
</details>

---

6. Can we modify the ServiceNow email size limit?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
We cannot.You must use your own email infrastructure that supports larger emails if you want to change the email size restriction.

</blockquote>
  
</details>

---

7. If the same trigger is generating multiple notifications will all the notifications get sent?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
No, In this case only one notification with higher weight will get sent and other notifications will get ignored.

</blockquote>
  
</details>

---

8. How can the email notification recipient limit be changed?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
by modifying the glide.email.smtp.max recipients system property.

</blockquote>
  
</details>

---

9. If in the notification recipient list we select an inactive user, will that user receive a notification?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
No. An inactive user will not receive the notification.

</blockquote>
  
</details>

---

10. Will a user get notification about a record on which he does not have access if he is added to the recipient list?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
As the system does not exclude the recipients based on access constraints, the user will be notified of the record event even if he does not have access to that record.

</blockquote>
  
</details>

---

11. Which subject would be displayed if you used an email template to generate an email and also typed text in the subject field?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
The text in the subject field will get displayed as it overrides the subject field of the email template.

</blockquote>
  
</details>

---

12. How can we hide the email watermark globally in servicenow?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
We have to create a new property inside sys_properties.list named glide.email.watermark.visible and have to set its value to false to hide the watermark globally.
But the watermark can only be hidden in HTML messages. The text version of the message will always have the watermark.

</blockquote>
  
</details>

--- 

13. How can we send document attachment with the email notification?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
To do this, we have two options. First, we can add a link to the attachments using a script or select the checkbox Include Attachments in Notification.

</blockquote>
  
</details>

--- 

14. How many ways we can trigger the notifications?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
We can trigger a notification by an event or we can insert or update a record.

</blockquote>
  
</details>

--- 

15. How we can add timezone in email notification?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
By setting glide.email.append.timezone to true, we can add the system time zone of the instance in outbound email notifications.

</blockquote>
  
</details>

--- 

16. How does ServiceNow recognize Inbound Emails?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
Via Watermark or InReplyTo email header. If These are not present, ServiceNow recognizes an email containing a prefix in the subject line.

</blockquote>
  
</details>

--- 

17. If you identify a domain as suspicious, how can you stop receiving email from that domain?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
By using email address filters, we can stop receiving emails from any suspicious domain. For this, we have to create an email filter of type Blacklist and add the domain from which we want to stop receiving emails.

</blockquote>
  
</details>

--- 

18. How can we call an email script in notification?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
We can call email scripts in notification by using the ${mail_script:&lt;nameofmailscript&gt;} syntax. 

</blockquote>
  
</details>

--- 

19. What are the different types of inbound email?


![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary><b> Show Answer</b></summary>
  
<blockquote>
  
Three different inbound email types are available: new, forward, and replay.

</blockquote>
  
</details>

--- 

