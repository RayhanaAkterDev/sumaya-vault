---
class: cse
title: 05 How does a linkage editor process an object program?
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
### How a Linkage Editor Processes an Object Program

A **linkage editor** processes an object program in several systematic steps to produce a complete and executable program, often allowing modular updates without full recompilation. Here’s how it works:

1. **Reading Object Modules:**  
    The linkage editor reads all the object modules (files) that are part of the program. These modules may be compiled separately and contain machine code, symbolic references, and relocation information.
    
2. **Symbol Resolution:**  
    The editor **resolves all external references** between the modules. For example, if one module calls a function defined in another module, the linkage editor matches the function call with the function definition.
    
3. **Address Relocation:**  
    Each module is designed with relative addresses. The linkage editor adjusts these **addresses to absolute memory locations**, ensuring that the program modules can work correctly when combined.
    
4. **Combining Modules:**  
    After resolving references and relocating addresses, the editor **merges all modules into a single executable program**. It arranges the code and data segments in memory appropriately.
    
5. **Library Inclusion:**  
    If the program uses standard or user-defined libraries, the linkage editor locates the required routines and **includes them in the final executable**, avoiding duplication of unused routines.
    
6. **Optional Updates or Replacements:**  
    One key advantage of a linkage editor is that it can **update or replace specific modules** without recreating the entire executable, which saves time in large programs.
    
7. **Generating Executable:**  
    Finally, the linkage editor outputs a **complete executable program**, ready to be loaded into memory by a loader or linking loader for execution.
    

**Example:**  
Suppose a program has `main.o`, `math.o`, and `io.o`. The linkage editor reads these object modules, resolves calls like `add()` in `main.o` to `math.o`, adjusts memory addresses, includes necessary library routines, and produces a single executable file. Later, if `math.o` is updated, the linkage editor can **replace only `math.o`** in the executable without touching `main.o` or `io.o`.