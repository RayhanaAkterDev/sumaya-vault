---
class: cse
title: 05 Discuss about different types of cohesion in the context of software design. Which type of cohesion is best?
course:
  - Software Engineering
chapter:
  - "ch3: Software Design Fundamentals"
semester: 6th
date: 2025-08-04
status: pending 🛑
importance: ⭐⭐⭐⭐⭐
tags:
  - board_2019
  - board_2021
---

### Cohesion in Software Design

Cohesion is the **degree to which the elements within a module are related**. High cohesion means a module focuses on a single task, making it easier to understand, maintain, and reuse. Low cohesion occurs when a module handles unrelated tasks, increasing complexity and reducing maintainability.

---

### Types of Cohesion

1. **Coincidental Cohesion**  
    Coincidental cohesion occurs when a module performs multiple unrelated tasks. The elements have little or no relationship with each other. This type of cohesion is weak and undesirable because it makes the module complex and difficult to maintain.
    
2. **Logical Cohesion**  
    Logical cohesion happens when a module performs a series of related tasks, but only one is executed based on some control or decision. Although the tasks are conceptually related, combining them in a single module reduces clarity and increases complexity.
    
3. **Temporal Cohesion**  
    Temporal cohesion arises when a module performs activities that are related in time, such as initialization or cleanup tasks. While better than coincidental cohesion, it still mixes tasks that are not logically connected by functionality.
    
4. **Procedural Cohesion**  
    Procedural cohesion occurs when a module performs a sequence of steps that must be executed in a specific order. The tasks are related by the control flow rather than the purpose, making it moderately cohesive.
    
5. **Communicational Cohesion**  
    Communicational cohesion exists when the elements of a module operate on the same data or contribute to the same output. Modules with this cohesion are focused and more maintainable than those with procedural or temporal cohesion.
    
6. **Functional Cohesion**  
    Functional cohesion is achieved when all elements of a module work together to perform a single well-defined task. This is the strongest and most desirable type of cohesion because it maximizes clarity, maintainability, and reusability.
    
7. **Sequential Cohesion**  
    Sequential cohesion occurs when the output of one part of the module serves as input to another part. This type is stronger than procedural cohesion but not as strong as functional cohesion.
    

---

### **Best Type of Cohesion**

**Functional cohesion** is considered the best type because each module performs a single, well-defined task. High functional cohesion leads to modules that are easier to understand, test, maintain, and reuse, resulting in a more robust and modular software system.