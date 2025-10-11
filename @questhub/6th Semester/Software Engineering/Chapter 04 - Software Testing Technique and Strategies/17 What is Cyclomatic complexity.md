---
class: cse
title: 17 What is cyclomatic complexity?
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

## Cyclomatic Complexity

Cyclomatic complexity is a **software metric** that measures the **complexity of a program’s control flow** by counting the number of **linearly independent paths** through the code or a program module.  It was introduced by **Thomas J. McCabe in 1976**. This metric helps in assessing how **complex, testable, and maintainable** a program is.

**Purpose / Importance:**

1. **Measures Code Complexity:** Higher cyclomatic complexity indicates **more complex code** with many decision points, loops, or branches.    
2. **Guides Testing Effort:** It helps determine the **minimum number of test cases** needed for **full branch coverage**.    
3. **Predicts Maintenance Difficulty:** Code with high complexity is **harder to understand, maintain, and modify**.    
4. **Helps Identify Risky Code:** Modules with high cyclomatic complexity are more prone to **errors or defects**.

---

**Calculation:**  

Cyclomatic complexity (CC) can be calculated using the formula:

`CC = E - N + 2P`

Where:

- **E** = Number of edges in the control flow graph    
- **N** = Number of nodes in the graph    
- **P** = Number of connected components (usually 1 for a single program)