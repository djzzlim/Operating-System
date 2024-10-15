# CPU Scheduling

## Design and Implementation of Short-Term Scheduler

![Short-Term Scheduler](img/short_term_scheduler.drawio.png)

### Short-Term Scheduler Overview:
The **Short-Term Scheduler** (also known as the CPU Scheduler) is crucial in process management, responsible for selecting which process from the **Ready Queue** should be executed by the CPU next.

### Criteria for CPU Scheduling:

The short-term scheduler is designed with specific goals to optimize overall system performance. These goals include:

- **Maximizing CPU Utilization**: 
  - Keeping the CPU busy as much as possible, reducing idle time.
  
- **Maximizing Throughput**: 
  - Increasing the number of processes that complete their execution per unit time.

- **Maximizing Efficiency**: 
  - Ensuring the system’s resources are used effectively and without waste.

- **Minimizing Waiting Time**:
  - Reducing the amount of time a process spends waiting in the Ready Queue before it is given CPU time.

- **Minimizing Turnaround Time**:
  - Lowering the total time taken from submission of a process until its completion.

- **Minimizing Response Time**:
  - Particularly important for interactive systems, response time refers to the time it takes for a system to start processing requests after they have been submitted.

### Function of Short-Term Scheduler:

The main function of the short-term scheduler is to:

- **Select a process from the Ready Queue** and allocate it to the CPU for execution based on the chosen scheduling algorithm.

---

## Process Times and Scheduling Concepts

### 1. Arrival Time:
- The time at which a process enters the **Ready Queue** for the first time.

### 2. Waiting Time:
- The total time a process spends **waiting** in the Ready Queue before being assigned CPU time.

### 3. Burst Time:
- The time a process spends **running** on the CPU. This is the actual execution time.

### 4. I/O Burst Time:
- The time a process spends **waiting** for an I/O operation in the **Blocked State**.

    ### Note:
    - In most modern operating systems, when a process initiates an I/O operation, it doesn’t handle the operation itself.
    - Instead, it **initiates** the I/O operation and then enters a **Blocked State**.
    - The operating system handles the actual I/O on the process's behalf.

### 5. Completion Time:
- The time at which a process finishes its execution.

### 6. Turnaround Time:
- The total time spent by a process from entering the system (New) to its completion (Terminate).
  
  **Formula:**  
  $$
    L = \text{Completion Time of Last Process} - \text{Arrival Time of First Process}
$$

- **Waiting Time** can be derived as:  
  $$
    \text{Throughput} = \frac{\text{Number of Processes Completed}}{\text{Schedule Length (L)}}
$$

### 7. Schedule Length:
- The total time taken to complete all **n processes** as per a given schedule.

  **Formulas and Observations:**
  - Number of schedules possible with **n processes**:
    - **Non-preemptive** case: \(n!\) (Factorial)
    - **Preemptive** case: **Infinity** (due to constant process interruptions)

  - **Important Relationships**:
    - Adding the **Turnaround Time** of all processes results in a value greater than the Schedule Length (L).
    - Adding the **Burst Time** of all processes includes I/O Burst Time as well.

  **Schedule Length Formula:**  
  \[
  L = \text{Completion Time of Last Process} - \text{Arrival Time of First Process}
  \]

  **Throughput:**  
  \[
  \text{Throughput} = \frac{\text{Number of Processes Completed}}{\text{Schedule Length (L)}}
  \]

## Dispatcher and Context Switching Time:
- **Context Switching Time** and **Scheduling Overhead** is often referred to as **Dispatch Latency**.
- For simplicity, **loading time** (the time the dispatcher takes to load the Process Control Block (PCB) from the Ready Queue onto the CPU) is included in context switching time.
