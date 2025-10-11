---
class: cse
title:
course: Software Engineering
chapter:
  - "ch5: Software Management and Maintenance Technique"
semester: 6th
date: 2025-09-09
status: pending 🛑
importance: ⭐⭐⭐⭐⭐
tags:
  - board_2017
  - board_2018
  - board_2020
  - board_2021
---
### COCOMO Model

COCOMO (Constructive Cost Model) is a quantitative and algorithmic model used to **estimate the effort, cost, and schedule required to develop a software project**. It calculates the development effort based on the size of the software (measured in thousands of lines of code, KLOC) and considers other project-specific attributes such as team experience, software complexity, and hardware constraints. The model helps project managers plan resources, assign tasks, and control the development process efficiently. By providing systematic estimates, COCOMO reduces uncertainty in project planning and supports decision-making throughout the software lifecycle.

**Types of COCOMO Models:**

1. **Basic COCOMO:** Provides a rough estimate of effort and cost using only software size. Projects are classified as organic (small, simple, with an experienced team), semi-detached (medium complexity with mixed team experience), or embedded (large, complex, tightly constrained projects).
    
2. **Intermediate COCOMO:** Offers improved accuracy by including cost drivers such as product reliability, complexity, personnel experience, and hardware requirements, which adjust the effort estimate.
    
3. **Detailed COCOMO:** Provides a highly refined estimate by applying cost drivers to individual modules of the software and factoring in development phases, producing precise predictions of effort, schedule, and resource allocation.
    

**Example:**  
For a hospital management system estimated at 50 KLOC, the basic COCOMO model might estimate the development effort as approximately 188 person-months for an organic project. Using the intermediate or detailed COCOMO models, the estimate would be adjusted to account for factors like team experience, hardware limitations, and required reliability, resulting in a more accurate prediction of resources and schedule.