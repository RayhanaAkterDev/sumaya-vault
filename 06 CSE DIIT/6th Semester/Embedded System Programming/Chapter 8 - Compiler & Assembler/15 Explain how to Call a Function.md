---
class: cse
title: 15 Explain how to Call a Function?
course: Embedded System Programming
chapter:
  - "ch8: Compiler & Assembler"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - ESP/Ch8
---
## Explain How to Call a Function

To **call a function** means to invoke its execution from another part of the program. There are **different types of function calls** in embedded system programming:

1. **Direct Call:**  
    A direct call is the simplest and most common method, where the function is invoked explicitly by its **name** in the program. The control of execution **jumps to the function**, executes its code, and then returns to the point where it was called. This is straightforward and easy to understand, making it suitable for **most standard tasks** in embedded systems, such as reading sensor data or performing simple calculations.
    
    **Example:**
    
    ```c
    int result = add(5, 10);  // calling the function 'add'
    ```

---

2. **Indirect Call (Using Pointers):**  
	An indirect call uses a **pointer to a function** to invoke it. This allows the program to **dynamically decide at runtime which function to execute**, which is useful in **embedded systems** for event-driven programming, callbacks, or implementing state machines. Function pointers make the program flexible and modular, especially when different behaviors need to be selected based on conditions.
	
	**Example:**
	
	```c
    int (*funcPtr)(int, int) = add;
	int result = funcPtr(5, 10);
    ```

---

3. **Recursive Call:**  
	In a recursive call, a function **calls itself** either directly or indirectly. This is particularly useful for solving problems that can be **broken into smaller, similar subproblems**, like computing factorials, Fibonacci numbers, or traversing tree-like data structures. Embedded systems use recursion cautiously due to **limited stack memory**, but it is still valuable for tasks that have repetitive, nested patterns.  
	
	**Example:**
	
	```c
	int factorial(int n) {
    if (n == 0) return 1;
    return n * factorial(n - 1);  // Recursive call
	}
	```

---

4. **Callback or System-Triggered Call:**  
	In embedded systems, a function can be called **automatically by the system**, rather than directly by the programmer. Examples include **interrupt service routines (ISRs)** or **timer callbacks**. These functions are triggered by hardware or system events, making them essential for real-time operations, responding to external signals, or handling periodic tasks.  
	
	**Example:**
	
	```c
	void timerISR() {
    // Code executed when timer overflows
	}
	```