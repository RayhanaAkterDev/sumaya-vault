---
class: cse
title: 20 Write down pros and cons of top down integration testing.
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
  - board_2019
  - board_2020
---

**Top-Down Integration Testing** is an approach where the **top-level modules are tested first**, and lower-level modules are integrated and tested step by step using **stubs** to simulate the lower modules not yet integrated.

### **Pros**

1. **Early validation of major control flows:** Top-level modules control the system’s flow, so testing them first ensures critical paths work early.
    
2. **Simplifies debugging:** Since modules are integrated incrementally from top to bottom, locating defects is easier.
    
3. **Early prototype availability:** Provides a working version of the main system early for stakeholder review.
    
4. **Supports incremental development:** Encourages systematic development and testing of modules.
    
5. **Focus on key modules first:** High-level, decision-making modules are prioritized, ensuring core functionality works.
    
6. **Improves requirement verification:** Top-level modules often correspond to key requirements, so verifying them first helps catch requirement errors early.
    
7. **Encourages proper design:** Forces developers to have a clear top-down design before implementation.
    
8. **Better integration flow:** Integration proceeds in a logical order, reducing chaos during module integration.
    

---

### **Cons**

1. **Requires stubs for lower modules:** Extra effort is needed to create stubs for modules not yet implemented.
    
2. **Lower-level modules tested late:** Bugs in lower-level modules may be detected only after significant top-level testing.
    
3. **Incomplete early testing:** Some defects in lower modules or detailed functionality may be missed initially.
    
4. **Complex stub creation for complex modules:** Designing accurate stubs for large modules can be difficult.
    
5. **Interface issues detected late:** Problems in interactions between lower and higher modules may appear late in the process.
    
6. **Not suitable for bottom-critical systems:** Systems where lower-level modules are essential early may not benefit from this approach.
    
7. **Extra maintenance for stubs:** As development progresses, stubs must be updated or removed, increasing maintenance work.
    
8. **May require more planning:** Detailed top-down planning is needed before starting integration, which can slow the initial testing phase.