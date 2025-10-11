---
class: cse
title: 15 Describe the rules to beat OF DFD with examples.
course: Software Engineering
chapter:
  - "ch3: Software Design Fundamentals"
semester: 6th
date: 2025-09-05
status: pending 🛑
importance: ⭐⭐⭐⭐
tags:
  - board_2017
  - board_2019
---

### **Rules to Create a DFD**

> NOTE: _see exam kit page no. 68_

A **Data Flow Diagram (DFD)** represents the flow of data within a system, showing how inputs are transformed into outputs through various processes. To ensure clarity, accuracy, and effectiveness, certain rules should be followed when creating a DFD.

1. **Identify External Entities**  
    Clearly define all sources and destinations of data outside the system, ensuring each entity interacts with the system only through data flows.
    
2. **Define Processes Clearly**  
    Each process should have a unique identifier and name that clearly describes its function. A process must transform incoming data into meaningful output.
    
3. **Show Data Flows Correctly**  
    All data flows should be named to indicate the information being transferred, connecting entities, processes, and data stores logically.
    
4. **Include Data Stores**  
    Represent all storage points for data within the system, ensuring data flows pass through processes rather than connecting external entities directly to data stores.
    
5. **Maintain Consistency Across Levels**  
    The Level 0 DFD should present the system as a single process interacting with external entities, while Level 1 and beyond should break the system into sub-processes without altering the overall data flow structure.
    
6. **Use Symbols Properly**  
    Processes should be represented by circles or ovals, data stores by rectangles, external entities by squares, and arrows for data flows to maintain standard notation and avoid confusion.
    
7. **Ensure Logical Flow**  
    Data should move logically from external entities to processes, between processes, and to data stores, avoiding unnecessary loops or illogical paths.
