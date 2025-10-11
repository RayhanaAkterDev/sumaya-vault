---
class: cse
title: 18 How to compute the cyclomatic complexity in order to find the number of independent paths with examples.
course:
  - Software Engineering
chapter:
  - "ch4: Software Testing Technique and Strategies"
semester: 6th
date: 2025-09-06
status: pending 🛑
importance: ⭐⭐⭐⭐⭐
tags:
  - board_2019
  - board_2021
---

Cyclomatic complexity is a **software metric** used to measure the **complexity of a program**. It helps determine the **number of independent paths** in the program, which in turn tells how many test cases are needed for **full branch coverage**.

---

### **Formula to Compute Cyclomatic Complexity**

There are **three common methods**:

1. **Using Control Flow Graph (CFG):**
    
    `V(G) = E − N + 2`
    
    Where:
    
    - `V(G)`= Cyclomatic Complexity        
    - `E` = Number of edges in the CFG
    - `N` = Number of nodes in the CFG

	**Steps to Compute Using CFG**

	1. Draw the **Control Flow Graph (CFG)** of the program.    
	2. Count **nodes (N)** → Each block of code.    
	3. Count **edges (E)** → Each control flow connection between nodes.    
	4. Apply the formula: `V(G) = E − N + 2`

---

2. **Using Decision Points:**
    
    `V(G) = D + 1`
    
    Where:
    
    - `D` = Number of decision points (like `if`, `while`, `for`, `case`)
        
3. **Using Regions in CFG:**
    
    `V(G) = R`
    
    Where:
    
    - `R` = Number of regions (areas enclosed by edges in CFG)
        

---