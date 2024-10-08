# Process Concepts and States

### Process:
- A **process** is a program in execution.
- When a program is loaded from disk to main memory, it becomes a process.

### Program:
- A **program** refers to an instance of a file, such as `.exe`, that is executed by the system.
- A program consists of:
  - **Data**: Operands or variables that the program manipulates.
  - **Instructions**: Commands like `Load`, `Add`, `Store`, `Multiply`, `SVC`, `BSA`, etc.

### Relationship Between Process and Program:
- A **process** is something created when a program is executed.
- The **program** itself is just a file or script on disk.

![Difference between process and program](img/process_vs_program.drawio.png)

---

### Data in a Program:

- **Static Data**: Fixed size or known size.
  - Example: `int a;` where `a` takes up 2 bytes.
- **Dynamic Data**: Memory allocated at runtime.
  - Example: `int a[10];` where `a` takes up 20 bytes.

---

### Memory Allocation for Static Data:

- **When does memory allocation occur for static data?**
  - **Compile Time?**  
    No, during compile time, the compiler only checks for syntactic correctness and generates code. No memory allocation happens at this stage.
  
  - **What if the program is compiled but not run?**  
    It's possible to compile a program without running it, and no memory is allocated at this point. If memory were allocated at compile time, it would be a waste.

- **Correct Answer: Load Time**  
  Memory for static data is allocated during **load time**, which is before the program starts running. This is when the program is loaded from disk to memory for execution.

