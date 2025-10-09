---
class: cse
title: 14 What is Function?
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch8
---
### Function

A **function** is a **named, self-contained block of code** that performs a specific task or operation within a program. It allows a programmer to **encapsulate a set of instructions** that can be executed whenever needed, without rewriting the same code multiple times. Functions are essential for **modular programming**, as they break complex programs into smaller, manageable, and reusable units, improving readability, maintenance, and debugging. A function can **accept inputs**, known as **parameters**, to work with different data values and can **return an output** or result to the part of the program that called it. In embedded system programming, functions are particularly useful for handling repetitive tasks such as reading sensor data, controlling actuators, or performing calculations, enabling efficient and structured program design.

**Example:**  
In C language, a function to add two numbers:

```c
int add(int a, int b) {
    return a + b;
}
```

Here, `add` is a function that performs the task of adding two integers and returning the result.