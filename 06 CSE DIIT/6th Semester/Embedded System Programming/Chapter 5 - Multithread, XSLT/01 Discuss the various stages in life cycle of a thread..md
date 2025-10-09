---
class: cse
title: 01 Discuss the various stages in life cycle of a thread.
course: Embedded System Programming
chapter:
  - "ch5: Multithread, XSLT"
semester: 6th
date: 2025-09-13
status: pending 🛑
tags:
  - board_2022
---
# Life Cycle of a Thread

In embedded system programming and multithreaded applications, a **thread** is the smallest unit of execution within a process. Threads allow multiple tasks to run concurrently within the same program, sharing resources like memory while executing independently. Understanding the **thread life cycle** is essential for efficient multitasking, synchronization, and resource management.

---

## Stages in the Life Cycle of a Thread

1. **New (Created) Stage**  
    A thread is in the **new stage** immediately after being created using APIs such as `pthread_create()` in C or `Thread` class in Java. In this stage, the thread object exists, but it has not yet started execution. No system resources are allocated to the thread at this point except for the memory to store its state.
    
2. **Runnable Stage**  
    After the thread’s `start()` method is called, it enters the **runnable state**. The thread is now eligible for execution and waits in the ready queue for the CPU to schedule it. Being runnable does not guarantee immediate execution; it depends on the CPU scheduler and thread priority.
    
3. **Running Stage**  
    When the CPU selects a thread from the ready queue, it enters the **running stage**. The thread’s instructions are executed, and it actively performs its assigned task. Only one thread per CPU core can be in the running state at a time, while others remain in the runnable or waiting states.
    
4. **Blocked/Waiting Stage**  
    A thread can enter the **blocked or waiting state** if it is waiting for a resource, I/O operation, or a synchronization event (like acquiring a mutex or waiting on a condition variable). The thread remains idle until the event occurs or the resource becomes available, after which it moves back to the runnable state.
    
5. **Timed Waiting (Optional Stage)**  
    In some systems, threads can be in **timed waiting**, where they wait for a specific period (e.g., using `sleep()` or `wait(timeout)`). After the time expires, the thread automatically moves back to the runnable state if it hasn’t been activated earlier.
    
6. **Terminated (Dead) Stage**  
    Once a thread completes its task or is explicitly stopped, it enters the **terminated stage**. The thread releases its resources and cannot be restarted. Any attempt to restart a terminated thread will result in an error.
    

---

### Example / Use Case

In an **embedded system controlling a robotic arm**, multiple threads may be used:

- One thread handles **sensor data reading**,    
- Another thread controls **motor movement**,    
- A third thread manages **communication with a control panel**.    

Each thread moves through its life cycle independently: creation → ready → running → waiting for resources → completion → termination. Proper thread life cycle management ensures smooth multitasking and real-time performance in embedded systems.