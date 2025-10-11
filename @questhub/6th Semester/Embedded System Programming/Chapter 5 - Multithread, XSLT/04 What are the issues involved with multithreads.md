---
class: cse
title: 04 What are the issues involved with multithreads?
course: Embedded System Programming
chapter:
  - "ch5: Multithread, XSLT"
semester: 6th
date: 2025-09-13
status: pending 🛑
tags:
  - board_2021
---
## Issues Involved with Multithreading

While multithreading allows concurrent execution and improves efficiency, it also introduces several issues that need careful management. These issues primarily arise from threads sharing resources and running independently, which can lead to unpredictable behavior if not properly controlled.

---

### Main Issues in Multithreading

1. **Race Conditions** – When two or more threads access and modify shared data simultaneously without proper synchronization, the final result can become unpredictable or incorrect.
    
2. **Deadlocks** – This occurs when two or more threads are waiting for resources held by each other, causing them to be stuck indefinitely without progress.
    
3. **Starvation** – Some threads may never get CPU time if higher-priority threads continuously consume resources, leaving lower-priority threads waiting indefinitely.
    
4. **Synchronization Overhead** – Ensuring proper access to shared resources through locks, semaphores, or mutexes adds extra processing overhead, which can reduce the performance benefits of multithreading.
    
5. **Complex Debugging** – Multithreaded programs are difficult to debug because issues like timing errors, race conditions, or deadlocks may occur intermittently and are hard to reproduce.
    
6. **Memory Consistency Issues** – Since threads share memory, changes made by one thread may not be immediately visible to others due to caching, buffering, or CPU optimizations.
    
7. **Context Switching Overhead** – Although lighter than process switching, frequent thread context switches consume CPU cycles and may degrade system performance if not managed properly.
    
8. **Resource Contention** – Multiple threads competing for the same CPU, memory, or I/O resources can lead to delays, bottlenecks, or inefficient utilization of system resources.
    
9. **Security Risks** – Improper handling of shared memory or resources can lead to vulnerabilities, especially in systems where threads have different privileges.