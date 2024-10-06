# Chapter 1 Q&A Section

## Q1
**Question:**  
Consider the following statements:

(i) Operating system implementation has architectural constraints.  
(ii) Operating system is a set of utilities.

Which of the following is true?  
(a) Only (i) is correct.  
(b) Only (ii) is correct.  
(c) Both (i) and (ii) are correct.  
(d) Neither (i) nor (ii) are correct.

**Answer:**  
**(c) Both (i) and (ii) are correct.**  
Explanation: Operating system implementation varies based on architectural constraints, such as those between mobile phones and PCs. Additionally, an operating system can be considered a set of utilities that simplifies application development.

---

## Q2
**Question:**  
Operating system working on strict deadlines are ________.

(a) Time-sharing OS.  
(b) Real-time OS.  
(c) Network operating system.  
(d) Centralized OS. 

**Answer:**  
**(b) Real-time OS.**  
Explanation: Examples include fire alarm systems, heart pacemakers, and missile control systems.

---

## Q3
**Question:**  
What is /must be the primary goal for hard real-time operating system?

(a) Robustness.  
(b) Reliability.  
(c) Efficiency.  
(d) Convenience.

**Answer:**  
**(c) Efficiency.**  
Explanation: While reliability is also a crucial characteristic of hard real-time operating systems, the primary goal is to ensure tasks are completed efficiently within strict deadlines, optimizing resource usage and performance.

---

## Q4
**Question:**  
Which of the following statement is/are correct?

(a) During Booting, OS is loaded into disk from main memory.  
(b) The area of memory where OS is stored, is known as system area.  
(c) Uni-programming can load and execute a single program in memory.  
(d) Uni-programming suffers from idleness of CPU.

**Answer:**  
**(b), (c), (d)**  
Explanation:  
- **(a)** is incorrect; during booting, the OS is loaded into main memory (RAM) from disk storage, not the other way around.
- **(b)** is correct because the operating system is stored in a specific area of memory, often referred to as the system area or kernel space.
- **(c)** is correct as uni-programming allows for loading and executing a single program at a time.
- **(d)** is correct since uni-programming can lead to CPU idleness when waiting for I/O operations to complete.  

---

## Q5
**Question:**  
Throughput is ________.

(a) Executing multiple programs in memory.  
(b) Total number of programs completed per unit time.  
(c) Total number of programs loaded into main memory.  
(d) None of the above.

**Answer:**  
**(b) Total number of programs completed per unit time.**   
Explanation: Throughput measures the efficiency of a system by quantifying how many processes or programs are completed within a specific time frame. A higher throughput indicates better performance and resource utilization.

---

## Q5
**Question:**  
Throughput is ________.

(a) Executing multiple programs in memory.  
(b) Total number of programs completed per unit time.  
(c) Total number of programs loaded into main memory.  
(d) None of the above.

**Answer:**  
**(b) Total number of programs completed per unit time.**   
Explanation: Throughput measures the efficiency of a system by quantifying how many processes or programs are completed within a specific time frame. A higher throughput indicates better performance and resource utilization.

---

## Q6
**Question:**  
Pre-emptive processes have ________.

(a) Forceful deallocation.  
(b) Better response time.  
(c) Both (a) and (b).  
(d) None of the above.

**Answer:**  
**(c) Both (a) and (b).**  
Explanation: Pre-emptive processes can be interrupted and resumed later, allowing for forceful deallocation of resources. This leads to better response times, especially in systems that prioritize quick task switching and responsiveness to user input.

---

## Q7
**Question:**  
Consider the following statements:

(i) Non-preemptive process can lead to starvation.  
(ii) Non-preemptive process has good response time.  
(iii) Non-preemptive process can release CPU voluntarily.  

Which of the following is correct?  
(a) (i) and (ii) are correct.   
(b) (ii) and (iii) are correct.     
(c) (i) and (iii) are correct.  
(d) All (i), (ii) and (iii) are correct.

**Answer:**  
**(c) (i) and (iii) are correct.**  
Explanation: Non-preemptive processes can lead to starvation, especially if higher-priority processes continuously take over the CPU. They can also voluntarily release the CPU when they finish execution or when they wait for I/O. However, non-preemptive processes generally have poorer response times compared to preemptive processes.

---

## Q8
**Question:**  
Function of operating system includes ________.    

(a) Resource Management.   
(b) Reliability.     
(c) Security.  
(d) Control over system performance.

**Answer:**  
**(a), (c), (d)**  
Explanation: The functions of an operating system primarily include resource management, ensuring security, and controlling system performance. While reliability is important, it is often seen as an aspect of the operating system's quality rather than a direct function.

---