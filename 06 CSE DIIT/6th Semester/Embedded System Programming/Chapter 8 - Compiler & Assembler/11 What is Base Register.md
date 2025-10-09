---
class: cse
title: 11 What is Base Register?
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch8
---
### Base Register

A **base register** is a special processor register used to hold the **starting address of a memory block or segment** in computer memory. It is primarily used in **relative or indexed addressing** schemes, where instructions specify memory locations using an **offset** rather than an absolute address. The value stored in the base register is added to this offset to calculate the **effective address** of the memory location that the CPU needs to access. This approach allows programs to be **relocatable**, meaning they can execute correctly even if loaded at different memory locations, since only the base register needs to be updated rather than all memory addresses in the program. Base registers are commonly used in **assembly language programming, operating systems, and dynamic memory management**, providing efficient, flexible, and compact memory addressing.

**Example:**  
If a base register contains the address `2000` and an instruction specifies an offset of `150`, the CPU calculates the effective memory address as `2000 + 150 = 2150`. The data at memory location `2150` is then accessed or manipulated as required by the program.