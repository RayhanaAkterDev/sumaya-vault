---
class: cse
title: 07 Define cohesion and coupling in the context of modularity.
course:
  - Software Engineering
chapter:
  - "ch3: Software Design Fundamentals"
semester: 6th
date: 2025-08-04
status: pending 🛑
importance: ⭐⭐⭐
tags:
  - board_2018
---

### Cohesion

Cohesion refers to the degree to which the elements within a single module work together to accomplish a specific task. In the context of modularity, a highly cohesive module focuses on a single responsibility, which makes it easier to understand, develop, test, and maintain. For example, a module designed solely for calculating employee salaries exhibits high cohesion because all its functions are related to one well-defined purpose. High cohesion also improves reusability, as the module can be used independently in other parts of the system.

### Coupling

Coupling refers to the degree of interdependence between different modules. In modular systems, low coupling is preferred because it allows modules to operate independently, reducing the effect of changes in one module on others. For example, if a payroll module relies only on the input data provided by the HR module, without directly accessing its internal data, the modules are loosely coupled. Low coupling improves flexibility, maintainability, and makes the system easier to modify or extend.
