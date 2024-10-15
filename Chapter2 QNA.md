# Chapter 2 Q&A Section

## Q1
**Question:**  
Let's say:

- t1 = User to Kernel Mode Switch Time  
- t2 = Process Switch Time  

Which one is bigger?

**Answer:**  
**t2 > t1**

**Explanation:**  
Process switching involves more overhead than simply switching modes because it requires:
- **Saving and restoring the process state** (including the Process Control Block or PCB).
- **Context switching**, which involves switching between processes, whereas a user-to-kernel mode switch involves fewer steps as it's mainly about switching the CPU's privilege level.
