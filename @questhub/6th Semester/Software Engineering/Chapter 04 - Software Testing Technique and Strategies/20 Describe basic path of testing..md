---
class: cse
title: 20 Describe basic path of testing.
course:
  - Software Engineering
chapter:
  - "ch4: Software Testing Technique and Strategies"
semester: 6th
date: 2025-09-06
status: pending 🛑
tags:
  - SE/Ch4
---

## Basic Path Testing**

**Basic path testing** is a **white-box testing technique** in software engineering that focuses on **testing all possible independent paths in a program**. The goal is to ensure that **every statement and decision in the code is executed at least once**, which helps in detecting errors in program logic, loops, and decision constructs. This technique is based on **cyclomatic complexity**, which determines the **number of independent paths** that must be tested.

### Steps in Basic Path Testing

1. **Develop the Control Flow Graph (CFG):** Draw a graph representing the program with nodes for each block of code and edges showing the flow of control. This helps visualize all possible execution paths.
    
2. **Calculate Cyclomatic Complexity (V(G)):** Use the formula `V(G) = E − N + 2` or `V(G) = D + 1` to determine the number of independent paths in the program. Here, EEE is the number of edges, NNN is the number of nodes, and DDD is the number of decision points.
    
3. **Identify Independent Paths:** Select paths through the program so that each path introduces at least one new edge or node that is not included in other paths.
    
4. **Design Test Cases:** Create test cases that execute each independent path at least once to ensure all possible flows of control are tested.
    
5. **Execute and Record Results:** Run the test cases and observe the program output to detect defects or logic errors in the code.

---

### Example

```c
void example(int x, int y) {
    if (x > 0) {
        if (y > 0)
            printf("Both positive");
        else
            printf("x positive, y non-positive");
    } else {
        printf("x non-positive");
    }
}
```

**Step 1: Decision Points**

- `if(x > 0)` → 1 decision    
- `if(y > 0)` → 1 decision    
- Total D = 2
    

**Step 2: Cyclomatic Complexity**

`V(G) = D + 1 = 2 + 1 = 3`

**Step 3: Independent Paths**

1. `x > 0` and `y > 0` → prints "Both positive"    
2. `x > 0` and `y <= 0` → prints "x positive, y non-positive"    
3. `x <= 0` → prints "x non-positive"    

✅ **Number of independent paths = 3**

- Test cases should cover all 3 paths.