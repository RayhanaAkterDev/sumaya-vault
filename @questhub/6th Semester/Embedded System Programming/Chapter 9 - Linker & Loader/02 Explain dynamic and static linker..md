---
class: cse
title: 02 Explain dynamic and static linker.
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
### Static Linker

A **static linker** is a software tool that combines all the object files and required library code into a **single executable** at **compile time**. It resolves all symbolic references between the object files by assigning actual memory addresses to functions and variables. The resulting executable is **self-contained** and can run independently without requiring external libraries. Static linking increases the size of the executable but allows faster execution since all code is already present. Static linking is commonly used in **embedded systems** and other environments where program reliability and execution speed are critical, as the executable does not depend on external files at runtime.

**Example:**  
If a program uses `printf` from the standard library, a static linker copies the machine code for `printf` into the executable, allowing the program to run without needing the library separately.

---

### Dynamic Linker

A **dynamic linker** is a software tool that links an executable to **shared libraries at runtime** rather than at compile time. The executable contains **references** to the library functions or modules, and the dynamic linker loads the required libraries into memory and resolves the references when the program runs. This approach produces **smaller executables**, allows multiple programs to share the same library, and enables updates to libraries without recompiling the program. Dynamic linking is widely used in modern operating systems and applications where **memory efficiency and maintainability** are important, allowing programs to take advantage of updated library versions automatically.

**Example:**  
If a program uses `printf` dynamically, the executable contains a reference to the shared library (e.g., `libc.so`). When the program runs, the dynamic linker loads the library and resolves the `printf` call.