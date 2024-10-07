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

## Q9
**Question:**  
Which of the following are allowed in kernel mode only? 

(a) Enabling / Disabling interrupt   
(b) Reading the system's time.     
(c) Context switching.  
(d) Clear the memory.

**Answer:**  
**(a), (c), (d)**  
Explanation:
- **(a) Enabling / Disabling interrupt**: This operation is a privileged action that can only be performed in kernel mode to prevent user applications from interfering with the system's interrupt handling.
- **(b) Reading the system's time**: This operation can typically be performed in both user mode and kernel mode, as most operating systems provide APIs for user applications to access system time without needing kernel privileges.
- **(c) Context switching**: This is a fundamental operation managed by the OS kernel to switch the CPU from one process or thread to another, ensuring that resources are allocated efficiently.
- **(d) Clear the memory**: This operation involves manipulating memory directly, which is restricted to kernel mode to maintain system stability and security. 

---

## Q10
**Question:**  
Which of the following is/are correct? 

(a) To switch from kernel mode to user mode, the mode bit should be changed to 1.   
(b) To switch from kernel mode to user mode, the mode bit should be changed to 0.     
(c) To switch from user mode to kernel mode, the mode bit should be changed to 1.  
(d) To switch from user mode to kernel mode, the mode bit should be changed to 0.

**Answer:**  
**(a), (d)**  
Explanation:
- **(a)** is correct because switching to user mode involves setting the mode bit to 1, indicating user mode.
- **(d)** is also correct since switching from user mode to kernel mode requires changing the mode bit to 0, indicating kernel mode.

---

## Q11
**Question:**  
Match the following: 

| Mode            | Characteristics |
|-----------------|-----------------|
| (i) User mode   | 1) Atomic       |
| (ii) Kernel mode| 2) Mode bit 0   |
|                 | 3) Privileged   |
|                 | 4) Preemptive   |

(a) (i)-2, 3; (ii)-1, 4     
(b) (i)-2, 1; (ii)-3, 4     
(c) (i)-2, 1, 4; (ii)-3     
(d) (i)-4; (ii)-1, 2, 3     

**Answer:**  
**(d) (i)-4; (ii)-1, 2, 3**  
Explanation:
- **User mode** is preemptive, meaning it can be interrupted by higher-priority processes.
- **Kernel mode** is associated with atomic operations (meaning they complete without interruption), uses mode bit 0, and has privileged access to system resources.

---

## Q12
**Question:**  
System call is used to access ________.

(a) Application functionality.  
(b) I/O functionality.     
(c) Operating system functionality.  
(d) None of these.

**Answer:**  
**(c) Operating system functionality.**  
Explanation:
System calls provide an interface for user applications to request services from the operating system, such as file management, process control, and communication.

---

## Q13
**Question:**  
Consider the following statements:

(i) Pre-defined functions start executing in kernel mode.
(ii) User-defined functions start executing in user mode.

Which of the following is correct?      
(a) Only (i) is correct.  
(b) Only (ii) is correct.     
(c) Both (i) and (ii) are correct.  
(d) Both (i) and (ii) are incorrect.

**Answer:**  
**(b) Only (ii) is correct.**  
Explanation:
User-defined functions execute in user mode, while pre-defined functions like system calls will switch to kernel mode when accessing operating system services.

---
## Q14
**Question:**  
Consider the following program:

```c
int main()
{
    fork();
    fork();
    fork();
    printf("GATE 2023");
    return 0;
}
```
How many times GATE 2023 will get printed?

**Answer:**  
**8**  
Explanation:
The `fork()` function creates a new process each time it is called. Each process can execute the subsequent `fork()` calls, leading to an exponential increase in the number of processes. 

After three `fork()` calls, there are \(2³ = 8\) processes, each printing "GATE 2023" once.

---
## Q15
**Question:**  
Mode bit is present in ________.

(a) Main Memory     
(b) Disk    
(c) Cache   
(d) Register    

**Answer:**  
**(d) Register**  
Explanation:
The mode bit is stored in a register (Program Status Word) within the CPU, which indicates whether the system is operating in user mode or kernel mode.

---

## Q16
**Question:**  
At system boot time, the hardware starts in ________.

(a) Kernel mode     
(b) User mode   
(c) Operating mode   
(d) Disk mode    

**Answer:**  
**(a) Kernel mode**  
Explanation:
At system boot time, the hardware initializes and operates in kernel mode to perform critical tasks necessary for loading the operating system and managing system resources.

---
[Back](Chapter1.md)