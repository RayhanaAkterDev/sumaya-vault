---
class: cse
title: 19 Write short notes on top-down and bottom-up integration testing.
course:
  - Software Engineering
chapter:
  - "ch3: Software Design Fundamentals"
semester: 6th
date: 2025-09-05
status: pending 🛑
importance: ⭐⭐⭐⭐
tags:
  - board_2017
  - board_2021
---

## **Top-Down and Bottom-Up Integration Testing**

Top-down and bottom-up integration testing are **strategies for combining and testing modules** after development to ensure the system works as intended.

1. **Top-Down Integration Testing**  
    Top-down integration testing starts by testing **high-level modules first**. Modules that are not yet implemented are simulated using **stubs**, which mimic the behavior of the missing modules. As testing progresses, lower-level modules are integrated one by one and tested along with the already tested high-level modules. This method allows early validation of the main control and communication flows, helping to detect design or logic errors at the top level. It is particularly useful when high-level modules are critical to the system’s core functionality. However, creating stubs for lower modules can be time-consuming, and defects in lower-level modules are detected later in the process.
    
2. **Bottom-Up Integration Testing**  
    Bottom-up integration testing begins by testing **low-level modules first**. These foundational modules are thoroughly tested individually, then progressively integrated to form higher-level modules. **Drivers** are often used to simulate the behavior of higher-level modules that are not yet developed. This approach ensures that the core modules work correctly before they are assembled into the full system. Bottom-up integration testing reduces the risk of propagating errors from lower modules to higher-level components and makes debugging easier for the base functionality. However, the main control flow is tested only after integrating the higher modules.
