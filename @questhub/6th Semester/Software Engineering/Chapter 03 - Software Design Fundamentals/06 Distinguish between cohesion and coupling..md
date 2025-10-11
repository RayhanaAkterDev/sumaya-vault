---
class: cse
title: 06 Distinguish between cohesion and coupling.
course:
  - Software Engineering
chapter:
  - "ch3: Software Design Fundamentals"
semester: 6th
date: 2025-08-04
status: pending 🛑
importance: ⭐⭐⭐⭐
tags:
  - board_2018
---

|Feature|**Cohesion**|**Coupling**|
|---|---|---|
|**Definition**|Cohesion refers to the degree to which the elements within a single module are related and work together to achieve a specific task.|Coupling refers to the degree of interdependence between different modules in a system.|
|**Focus**|Focuses on the **internal quality** of a module.|Focuses on the **interaction** between modules.|
|**Goal**|High cohesion is desired to make a module clear, maintainable, and reusable.|Low coupling is desired to reduce dependencies and make modules independent.|
|**Effect on Maintenance**|High cohesion makes the module easier to understand, test, and maintain.|High coupling makes the system harder to maintain, test, and modify.|
|**Nature**|Internal property of a module.|External property between modules.|
|**Example**|A module that only calculates salaries and nothing else has high cohesion.|If a module directly modifies variables of another module, it has high coupling.|
|**Change Impact**|Changes within a highly cohesive module usually have minimal effect on other modules.|Changes in a highly coupled module often require changes in dependent modules.|
|**Design Implication**|High cohesion encourages modular, understandable, and reusable code.|Low coupling encourages flexibility and easier integration of modules.|
|**Measurement**|Measured by how focused the tasks within a module are.|Measured by the number and strength of dependencies between modules.|