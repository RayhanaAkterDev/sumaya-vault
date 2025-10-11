---
class: cse
title: 04 What is linkage editor and linking loader?
course: Embedded System Programming
chapter:
  - "ch9: Linker & Loader"
semester: 6th
date: 2025-09-11
status: pending 🛑
importance: ⭐⭐⭐⭐⭐
tags:
  - board_2021
topic: Set 05 & 06
---
### **Linkage Editor**

A **linkage editor** is a software tool that performs the functions of a **linker** but allows **modifications to object files without recreating the original executable**. It combines multiple object files, resolves symbolic references, and handles relocation, similar to a linker, but it can also **update or replace modules in an existing executable**. This is particularly useful in large systems where only a part of the program needs to be changed, avoiding the need to recompile and relink the entire program.

**Example:**  
If a program has `main.o`, `math.o`, and `io.o`, and only `math.o` is updated, the linkage editor can **replace the old `math.o` code** in the executable without affecting `main.o` or `io.o`.

---

### **Linking Loader**

A **linking loader** is a software tool that combines **linking and loading** functions in a single step. It not only loads the program into memory but also resolves **symbolic references** and performs **relocation** at runtime. This is especially useful for **dynamic linking**, where object modules or shared libraries may not be available until the program runs. Linking loaders make programs more flexible and reduce memory usage since they allow **modular loading** of program components.

**Example:**  
When running a program that uses a shared library `math.so`, the linking loader loads the main executable and resolves the call to `add()` in the library while placing both in memory for execution.