---
class: cse
title: 07 List out the services that a system call can provide.
course:
  - Embedded System Programming
chapter:
  - "ch3: Active X"
semester: 6th
date: 2025-09-05
status: pending 🛑
tags:
  - ESP/Ch3
---

### Services Provided by System Calls

1. **Process Management**  
    System calls allow the creation, termination, and control of processes. They handle operations like starting a new process, scheduling, and managing process states. Examples include `fork()`, `exec()`, and `exit()` in Unix/Linux.
    
2. **File Management**  
    System calls provide operations for creating, opening, reading, writing, and deleting files. They also allow programs to manage file attributes and access permissions. Examples include `open()`, `read()`, `write()`, and `close()`.
    
3. **Device Management**  
    These calls allow programs to interact with hardware devices, such as reading from or writing to a disk, printer, or keyboard. Examples include `ioctl()` and `read()`/`write()` for devices.
    
4. **Information Maintenance**  
    System calls provide ways to retrieve or set system information, such as system time, user IDs, and resource usage statistics. Examples include `getpid()` and `alarm()`.
    
5. **Communication**  
    They support interprocess communication (IPC) by enabling data exchange between processes on the same system or over a network. Examples include `pipe()`, `shmget()`, and `msgsnd()`.
    
6. **Protection and Security**  
    System calls enforce access control by allowing programs to set permissions, authenticate users, and ensure secure access to resources. Examples include `chmod()` and `setuid()`.
