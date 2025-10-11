---
class: cse
title: 07 What is Loader?
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
### Loader

A **loader** is a component of the operating system responsible for **loading executable programs into main memory** so they can be run by the CPU. Its primary function is to **prepare the program for execution** by allocating memory space, setting up the **stack and heap**, and resolving any **dynamic references** in case of shared libraries or dynamically linked modules. The loader also handles **relocation**, adjusting memory addresses so that the program can execute correctly in the allocated memory area.

Loaders are essential because an executable file stored on disk cannot run directly; it must first be brought into memory and properly organized so the CPU can execute its instructions sequentially.

**Example:**  
When you run a program like `myprogram.exe`, the loader reads the executable file from disk, loads the code and data segments into memory, sets up the execution environment, and transfers control to the program’s entry point (usually the `main` function), allowing the program to run.