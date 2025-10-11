---
class: cse
title: 17 What do you mean by Process State?
course: Embedded System Programming
chapter:
  - "ch6: WWW, Kernel, ASP"
semester: 6th
date: 2025-09-13
status: pending 🛑
tags:
  - ESP/Ch6
---
## Process State

A **process state** refers to the **current status or condition of a process** in an operating system at any given time. It represents what the process is doing or waiting for during its lifecycle, from creation to termination. Operating systems keep track of process states to manage CPU scheduling, resource allocation, and execution efficiently. Each process moves through different states depending on events like CPU allocation, I/O operations, or completion of tasks.

---

### Common Process States

1. **New / Created** – The process is being created but has not yet been admitted to the ready queue.    
2. **Ready** – The process is loaded into main memory and waiting for CPU allocation to execute.    
3. **Running** – The process is currently being executed by the CPU.    
4. **Waiting / Blocked** – The process is waiting for some event or I/O operation to complete before it can proceed.    
5. **Terminated / Exit** – The process has completed execution or has been killed and is removed from the process table.    

---

✅ **Example:**  

Suppose you launch a text editor:

- Initially, the OS creates the process (**New**).    
- Once loaded into memory, it waits for CPU allocation (**Ready**).    
- While you type, the CPU executes the process (**Running**).    
- If it waits for a file to load from the disk, it goes into **Waiting**.    
- When you close the editor, the process ends (**Terminated**).