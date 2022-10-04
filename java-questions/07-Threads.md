1. What are Threads?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 A thread is a single sequential flow of control within a program.The real excitement surrounding threads is not about a single sequential thread. Rather, it’s about the use of multiple threads running at the same time and performing different tasks in a single program. 
 
</blockquote>
</details>

--- 

2. Tell us about Java Threads

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
Threads are basically the lightweight and smallest unit of processing that can be managed independently by a scheduler. Threads are referred to as parts of a process that simply let a program execute efficiently with other parts or threads of the process at the same time. Using threads, one can perform complicated tasks in the easiest way. It is considered the simplest way to take advantage of multiple CPUs available in a machine. They share the common address space and are independent of each other
 
</blockquote>
</details>

--- 

3. How do you make a thread in java?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 There are basically two ways of implementing thread in java as given below:

By Extending the Thread class
Example:

class ThreadingDemo extends Thread 
{   
  public void run() 
 {   
     System.out.println("My thread is in running state.");    
 } 
  public static void main(String args[]) 
 {   
    ThreadingDemo obj=new ThreadingDemo();  
        obj.start();  
  }  
} 

Output:

My thread is in running state.
By Implementing Runnable interface in Java
Example:

class ThreadingDemo implements Runnable 
{  
   public void run() 
 {  
      System.out.println("My thread is in running state.");  
  }  
    public static void main(String args[]) 
 {  
      ThreadingDemo obj=new ThreadingDemo();   
      Thread t=new Thread(obj);       
      t.start();  
 }   
} 

Output: 
My thread is in running state.

 
</blockquote>
</details>

--- 

4. What is the life cycle of a thread?

![Easy](https://github.com/revaturelabs/interviewquestions/blob/dev/ComplexityTags/simple%20(2).svg)

<details>
  <summary> <b>Show Answer</b></summary>
  
<blockquote>
 New
 Runnable
 Waiting
 Timed Waiting
 Terminated (Dead)
 
</blockquote>
</details>

--- 
