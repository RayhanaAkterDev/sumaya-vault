---
class: cse
title: 12 What is absolute loader? What are the types of loaders? Explain.
course: Embedded System Programming
chapter:
  - "ch9: Linker & Loader"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch9
---
### Absolute Loader

An **absolute loader** is the simplest type of loader that directly loads the object code into main memory at the fixed addresses specified in the program. It does not perform relocation or linking; instead, it assumes that the programmer or assembler has already assigned the correct memory addresses to instructions and data. Because of this, the absolute loader is fast and straightforward but offers no flexibility—if the program is to be run at a different memory location, it must be reassembled.

**Example:**  
If the object program specifies that an instruction must be placed at address `2000H`, the absolute loader loads it exactly at that location in memory without any modifications.

---

### Types of Loaders 

Loaders are generally classified into the following types:

1. **Absolute Loader**  
    An absolute loader loads the program into memory at the exact addresses defined in the object code. It is simple and fast but lacks flexibility since any change in the memory location requires reassembling the entire program.
    
2. **Relocating Loader**  
    A relocating loader allows a program to be placed into any memory location. It adjusts the addresses of instructions and data depending on the actual load location. This flexibility makes it possible to use the same program in different parts of memory without rewriting or reassembling the code.
    
3. **Linking Loader**  
    A linking loader not only loads the program into memory but also performs the linking process. It resolves external references between multiple object modules by assigning proper addresses to symbols and variables. This type of loader supports modular programming, where programs are divided into smaller modules that can be developed and compiled separately.
    
4. **Dynamic Loader**  
    A dynamic loader loads and links program modules at runtime instead of before execution. This allows programs to load only the modules or libraries they need at a particular time, saving memory and improving efficiency. It is widely used in modern operating systems for handling shared libraries or dynamically linked libraries (DLLs).