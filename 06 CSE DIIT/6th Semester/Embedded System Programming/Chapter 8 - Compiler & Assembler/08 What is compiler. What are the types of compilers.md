---
class: cse
title: 08 What is compiler? What are the types of compilers?
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch8
---
### Compiler

A **compiler** is a software program that translates the entire **high-level programming language code** (like C, C++, or Java) into **machine code or intermediate code** that a computer can execute. Unlike an interpreter, which executes the code line by line, a compiler analyzes the whole program, performs optimization, and generates an executable file. It acts as a bridge between human-readable code and CPU-executable instructions, ensuring the program runs efficiently on the target machine.

The main tasks of a compiler include **lexical analysis, syntax analysis, semantic analysis, code optimization, and code generation**. It also detects **errors** in the source code and reports them before execution.

---

### Types of Compilers (Detailed Explanation)

1. **Single-Pass Compiler:**  
    A single-pass compiler translates the entire source program into machine code in **one pass** from start to finish. It is faster and requires less memory, making it suitable for **small programs**. However, it has limitations in handling **forward references** (when a function or variable is used before being declared) and cannot perform complex optimizations.
    
2. **Multi-Pass Compiler:**  
    A multi-pass compiler reads the source code **multiple times**, with each pass performing a specific task. The first pass may handle **lexical and syntax analysis**, the next pass may handle **semantic analysis and intermediate code generation**, and the final pass generates **optimized machine code**. This type of compiler is more **powerful and flexible**, suitable for **large programs**, and can handle forward references and advanced optimization techniques efficiently.
    
3. **Cross Compiler:**  
    A cross compiler runs on one type of computer (host machine) but produces **machine code for a different type of computer (target machine)**. This is widely used in **embedded systems**, microcontrollers, or any situation where the target machine cannot run a compiler natively. For example, compiling code on a Windows PC to run on an ARM-based device.
    
4. **Bootstrap Compiler:**  
    A bootstrap compiler is written in the **same programming language** that it is designed to compile. For example, a C compiler written in C. This type of compiler is used to **improve or update** itself, and it helps in building a fully functional compiler from a simpler version.
    
5. **Just-In-Time (JIT) Compiler:**  
    JIT compilers translate high-level code into machine code **during program execution** rather than before running. This allows for **runtime optimization**, such as faster execution of frequently used code. JIT compilation is commonly used in **Java Virtual Machine (JVM)** and **.NET platforms**.
    
6. **Incremental Compiler:**  
    Incremental compilers compile **only the portions of the code that have changed**, instead of recompiling the entire program. This reduces compilation time significantly for **large projects** and is often used in modern development environments with frequent code updates.