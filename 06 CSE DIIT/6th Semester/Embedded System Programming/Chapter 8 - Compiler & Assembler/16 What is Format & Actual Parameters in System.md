---
class: cse
title: 16 What is Format & Actual Parameters in System?
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch8
---
### Format (Formal) parameter

Formal parameters, also called **format parameters**, are the **variables defined in a function’s definition** to receive input values when the function is called. They act as **placeholders** for the data that the function will process and define the **number, type, and order of inputs** expected by the function. Formal parameters exist only within the **scope of the function** and are used to manipulate or compute results based on the values passed by the caller. They are essential for making functions **generic and reusable**, as the same function can operate on different data without changing its definition.

**Example of Formal Parameters**

```c
int add(int x, int y) {  // x and y are formal parameters
    return x + y;
}
```

---

### Actual parameters 

Actual parameters, also called **arguments**, are the **real values or expressions provided by the calling program** to the function. These values are assigned to the formal parameters when the function is invoked. Actual parameters supply the **specific data** that the function uses for its computation, allowing the same function to produce different results depending on the input. They can be **constants, variables, or expressions**, giving flexibility to the program.


**Example of Actual Parameters**

```c
int a = 5, b = 10;
int result = add(a, b);  // a and b are actual parameters
```