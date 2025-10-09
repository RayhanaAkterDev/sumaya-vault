---
class: cse
title: 06 Define system call.
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

### Definition of System Call

A **system call** is a mechanism that allows a user-level program to request services from the operating system kernel. Since applications cannot directly access hardware or critical OS resources for security and stability reasons, system calls provide a controlled interface to perform tasks such as file operations, process management, memory allocation, and communication.

In simple terms, a system call acts as a **bridge between user applications and the operating system**, enabling programs to execute operations that require privileged access.

---

**Example:** Functions like `open()`, `read()`, `write()`, and `fork()` in Unix/Linux are all system calls that allow programs to interact safely with the underlying OS.