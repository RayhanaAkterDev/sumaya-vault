---
class: cse
title: 13 What is Data Protection directive?
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch8
---
### Data Protection Directive

A **Data Protection Directive** in assembly language is an **assembler directive used to control access to data**, ensuring that certain sections of memory or variables are **protected from unauthorized modification** during program execution. It instructs the assembler to mark specified data areas as **read-only**, **write-protected**, or **restricted**, helping prevent accidental overwriting of critical data, constants, or system variables.

These directives are particularly useful in programs where **data integrity and security** are important, such as in operating systems, embedded systems, or applications handling sensitive information. By using data protection directives, the programmer can define sections of memory that the CPU cannot modify, allowing only reading operations or controlled access through proper instructions.

**Example:**  
In some assemblers, the directive `EQU` can be used to define a constant value that **cannot be changed** throughout the program:

```nginx
PI EQU 3.1416
```

Here, `PI` is assigned a fixed value, and the assembler prevents it from being altered elsewhere in the code, providing **data protection**.

In essence, a **data protection directive** helps maintain the **accuracy, reliability, and safety** of critical data within a program.
