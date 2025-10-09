---
class: cse
title: 10 Explain how Machine-Independent Loader Features Automatic Library Search Loader Options?
course: Embedded System Programming
chapter:
  - "ch9: Linker & Loader"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch9
---
### Machine-Independent Loader Features: Automatic Library Search and Loader Options

A **machine-independent loader** is designed to provide flexibility and portability by including features that are not tied to any specific hardware architecture. Two important features of such loaders are **automatic library search** and **loader options**, which help make program loading easier, more efficient, and user-controlled.

---

#### 1. Automatic Library Search

Automatic library search is a feature where the loader automatically searches for and includes necessary routines from standard libraries or user-defined libraries during program loading. If a program refers to an external function or subroutine that is not found in the object file, the loader looks into the specified libraries, locates the required routine, and links it with the program.

This saves programmers from manually specifying all library routines, reduces errors, and speeds up program development.

**Example:**  
If a program calls `printf()` in C but the function is not present in the object file, the loader automatically searches the C standard library, finds the definition, and links it.

---

#### 2. Loader Options

Loader options are **special control instructions** that allow the programmer to influence the loader’s behavior during program loading. These options are specified either in the source code or as external commands. They give flexibility in deciding how the program is loaded into memory.

Some common loader options include:

1. **Library Path Option** – directs the loader to search in user-specified directories for library routines.    
2. **Include/Exclude Option** – allows inclusion or exclusion of certain routines while linking.    
3. **Trace Option** – provides step-by-step information on how loading and linking are carried out, useful for debugging.    
4. **Relocation Option** – allows the user to specify the starting address in memory where the program should be loaded.    

**Example:**  
If a programmer specifies a relocation option `LOAD 2000H`, the loader places the program starting from memory address `2000H` instead of the default location.