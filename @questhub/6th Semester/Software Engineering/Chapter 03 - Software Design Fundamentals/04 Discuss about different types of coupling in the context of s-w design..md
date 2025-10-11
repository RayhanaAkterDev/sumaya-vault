---
class: cse
title: 04 Discuss about different types of coupling in the context of s/w design.
course:
  - Software Engineering
chapter:
  - "ch3: Software Design Fundamentals"
semester: 6th
date: 2025-08-04
status: pending 🛑
importance: ⭐
tags:
  - board_2022
---

### Coupling in Software Design

Coupling is the degree of interdependence between software modules. Lower coupling is preferred because it makes modules more independent, easier to maintain, and less prone to errors. Higher coupling increases dependencies, making the system harder to modify and extend.

---

### Types of Coupling

1. **Content Coupling**  
    Content coupling occurs when one module directly accesses or modifies the internal data or logic of another module. This creates a strong dependency, so any change in the affected module can easily break the dependent module. Content coupling is considered highly undesirable in software design.
    
2. **Common Coupling**  
    Common coupling arises when multiple modules share the same global data. While it allows different modules to communicate, it can lead to unintended side effects and makes debugging and maintenance more difficult.
    
3. **External Coupling**  
    External coupling happens when modules depend on external systems, devices, or file formats. For example, if a module relies on the structure of an external configuration file, changes in that file can impact the module. Some level of external coupling is often unavoidable.
    
4. **Control Coupling**  
    Control coupling occurs when one module controls the behavior of another by passing control information, such as flags or commands. While sometimes necessary, excessive control coupling increases interdependence and can reduce modularity.
    
5. **Stamp (Data-Structured) Coupling**  
    Stamp coupling happens when modules share a composite data structure but only use a portion of it. This creates unnecessary dependencies and reduces the independence of modules, making maintenance harder.
    
6. **Data Coupling**  
    Data coupling is the lowest form of coupling, occurring when modules share only the data necessary for the operation through parameters. This type is highly desirable because it keeps modules independent, improving maintainability and flexibility.
