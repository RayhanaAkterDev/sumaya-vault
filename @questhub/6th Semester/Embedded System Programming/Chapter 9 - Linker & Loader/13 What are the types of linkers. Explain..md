---
class: cse
title: 13 What are the types of linkers? Explain.
course: Embedded System Programming
chapter:
  - "ch9: Linker & Loader"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch9
---
### Types of Linkers

A **linker** is a program that joins object files from a compiler or assembler into a single executable. It connects function calls and variables across files, assigns memory addresses, and prepares the program to run. There are two main types: **static linker** and **dynamic linker**.

---

1. **Static Linker**  
    A static linker performs the linking process at **compile time**. It takes all the object files and the required library routines, combines them into a single executable, and assigns final memory addresses. Once the program is created, all the necessary code is already included in the executable file. This makes execution faster since no linking is required at runtime. However, the executable becomes large because it contains all the library routines, even if only a small part of them is used.
    

**Example:**  
If a program uses the `math` library for only one function, such as `sqrt()`, the static linker will include the entire library code in the executable file.

---

2. **Dynamic Linker**  
    A dynamic linker performs the linking process at **runtime** instead of compile time. In this case, the main program and required library routines are kept separately. When the program is executed, the dynamic linker loads the necessary library routines into memory and links them with the program on demand. This reduces the size of the executable file and saves memory since common libraries can be shared by multiple programs at the same time. However, it may introduce a slight delay during program execution because linking happens at runtime.
    

**Example:**  
In modern operating systems, when a program uses `printf()` from the C standard library, the function is linked dynamically through a shared library file like `libc.so` (Linux) or `msvcrt.dll` (Windows).