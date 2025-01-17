## Technical

1. What is Deadlock condition?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)


<details><summary> Show Answer </summary>

<blockquote>

- When two or more threads are in block state waiting for one another to release the resource that they are having.

- For example, let us assume, we have two processes A1 and A2. Now, process A1 is holding the resource R1 and is waiting for the resource R2. At the same time, the process A2 is having the resource R2 and is waiting for the resource R1. So, no one is releasing any resource, both are waiting for each other to release the resource. This is called deadlock condition.

</blockquote>
</details>

---

2. Define about Starvation.

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary> Show Answer </summary>

<blockquote>

In Starvation, Threads are waiting for each other. But waiting time is not infinite after some interval of time, waiting thread gets the resources whatever is required to execute thread `run()` method.

</blockquote>

</details>

---

3. How to avoid deadlock in Java?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details><summary> Show Answer </summary>

<blockquote>

- We cannot completely avoid deadlock but can follow these measures to them

    - Avoid Nested Locks - avoid giving locks to multiple threads
    - Avoid Unnecessary Locks - lock is for important thread not for unnecessary threads.
    - Using Thread Join- use Thread.join with a maximum time that a thread will take to avoid a 
      situation where a thread waiting for other thread to relaese.

</blockquote>

</details>

---

4. How to detect the deadlock condition?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details><summary> Show Answer </summary>

<blockquote>

Deadlock situations can be detected by running the executable code on `cmd` and subsequently collecting the thread dump. If it occurs, the `cmd` will throw up a message. 


</blockquote>

</details>

---

5. How does Java handle starvation? 

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details><summary> Show Answer </summary>

<blockquote>

 -  Using the below methods we can remove the starvation.

`Thread.yield()`-When the thread in the process after releasing the lock gets a fair chance to occupy the C.P.U. and can get time to complete its execution till the original thread again gets the control over the C.P.U.
`Thread.sleep()` -Method to given chance to other Threads for execution.

 </details>

</blockquote>

--- 
6. What may be the reason of deadlock situation?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details><summary> Show Answer </summary>

<blockquote>

Synchronized keyword is the only reason for deadlock situation, which allows only one thread can access the resource at a given point in time. 

</details>

</blockquote>

---

7. Difference between deadlock and starvation 

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details><summary> Show Answer </summary>
<blockquote>
    
| **Deadlock** | **Starvation** |
|---|---|
| There are two threads waiting for each other to complete the task and none get executed | Due to high priority process, less priority process gets blocked |
| Processes block the resources | High priority processes are utilizing resources |

</blockquote>
</details>

---


8. Write a program to illustrate deadlock condition?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)

<details><summary> Show Answer </summary>

<blockquote>


``` java

class DeadlockSample extends Thread {
    static Thread mainThread;
    public void run()
    {
        System.out.println("Thread2 waiting for" +
                          " Thread1 completion");
        try {
            mainThread.join();
        }
        catch (InterruptedException e) {
            System.out.println("Thread2 execution" +
                                           " completes");
        }
    }
    public static void main(String[] args)
                   throws InterruptedException
    {
        DeadlockSample.mainThread = Thread.currentThread();
        DeadlockSample thread = new DeadlockSample();
 
        thread.start();
        System.out.println("Thread1 waiting for " +
                            "Thread2 completion");
        thread.join();
 
        System.out.println("Thread1execution" +
                                      " completes");
    }
}

```

</blockquote>

<details><summary> Explanation </summary>

<blockquote>

Here the thread1 will wait for thread2 to complete and thread2 will wait for thread1 to complete. Thus, the deadlock condition occurs.
</blockquote>
</details>

</details>

---

9. What is the difference between deadlock and starvation?

![Medium](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/Medium%20(2).svg)
<details><summary> Show Answer </summary>
<blockquote>
    
- Deadlock and starvation occurs when the processes requesting a resource have been waiting for a long time. 
- Deadlock occurs when each process holds a resource and waits for another resource which is in hold by other process. 
- In contrast, in starvation, the processes with high priorities continuously consume resources, holding low priority processes from using the resources.
</blockquote>
</details>
    
---
