---
class: cse
title: 06 What is dynamic linking editors?
course: Embedded System Programming
chapter:
  - "ch9: Linker & Loader"
semester: 6th
date: 2025-09-11
status: pending 🛑
importance: ⭐⭐⭐⭐⭐
tags:
  - board_2020
topic: Set 05 & 06
---
### Dynamic Linking Editor

A **dynamic linking editor** is a type of linkage editor that performs **linking of object modules or libraries at runtime** rather than at compile time. Unlike a static linker, which combines all object files and libraries into a single executable beforehand, a dynamic linking editor allows programs to **reference external modules or shared libraries** and resolves these references only when the program is loaded or executed.

This approach has several advantages: it produces **smaller executables**, allows **library updates without recompiling** the program, and enables multiple programs to **share common code** in memory, improving efficiency. Dynamic linking is especially important in **modern operating systems and embedded systems**, where programs frequently use shared libraries or modules that may be updated independently.

**Example:**  
If a program calls a math library function `sqrt()` dynamically, the executable contains a **reference to the shared library** (e.g., `libm.so`). When the program runs, the dynamic linking editor loads the library into memory and links the function call to its actual code at runtime.