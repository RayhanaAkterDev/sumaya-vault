---
class: cse
title: "08 What are the purposes of the following system calls - fork(), exit(), \rwait()"
course:
  - Embedded System Programming
chapter:
  - "ch3: Active X"
semester: 6th
date: 2025-09-05
status: pending 🛑
tags:
  - board_2021
---

### Purposes of Common System Calls

1. **fork()**  
    The `fork()` system call is used to create a new process by duplicating the calling process. The new process, called the **child process**, gets a separate memory space but initially contains a copy of the parent process’s data. Both parent and child processes execute concurrently, which enables multitasking in operating systems. `fork()` returns a value that allows the program to distinguish between the parent and the child process, helping in controlling the flow of execution. For example, after calling `fork()`, the parent process can continue to execute, while the child process can perform a different task like running a new program.

---

2. **exit()**  
    The `exit()` system call terminates the execution of a process. When a process calls `exit()`, all resources allocated to it, such as memory and file descriptors, are released back to the system. It also returns an **exit status** to the operating system, which can be used by the parent process or other programs to determine whether the process completed successfully or encountered an error. This ensures proper cleanup of resources and prevents resource leaks. For example, after completing a computation, a child process may call `exit(0)` to indicate successful termination.
---

3. **wait()**  
    The `wait()` system call is used by a parent process to pause its execution until one of its child processes terminates. It helps in **process synchronization**, ensuring that the parent can retrieve the exit status of the child before proceeding further. Without `wait()`, the parent might terminate before the child, leading to **zombie processes**. For example, in a program where a parent creates multiple child processes for parallel tasks, `wait()` allows the parent to know when each child has finished and handle its results appropriately.