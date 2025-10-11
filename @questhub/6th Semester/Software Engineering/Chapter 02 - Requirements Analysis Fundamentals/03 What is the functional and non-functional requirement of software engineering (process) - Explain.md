---
class: cse
title: 03 What is the functional and non-functional requirement of software engineering (process) - Explain
course: Software Engineering
chapter:
  - "ch2: Requirements Analysis Fundamentals"
semester: 6th
date: 2025-07-08
status: pending 🛑
tags:
  - SE/Ch2
  - board_2020
  - board_2018
---

# The functional and non-functional requirement of software engineering

In software engineering, **requirements** are essential to define what a system should do and how it should behave. They are mainly divided into two types  —
1. Functional Requirements
2. Non-Functional Requirements

## Functional Requirements

**Functional requirements** define the specific behavior or *main functions* of a software system. They describe what the system should do, including all the features, operations, and interactions users can perform. More specifically, functional requirements describe the system’s functions, the expected inputs, how those inputs are processed, and the corresponding outputs. In some cases, they may also clearly state what the system should not do.

##### Common Functional Requirements in Software Engineering

- The user shall be able to log in with **valid credentials** and perform searches on either the entire **data set** or a **selected subset**.
- The system shall provide an **appropriate viewer** to read or display the uploaded documents.
- Each record in the database shall have a **unique identifier** to distinguish it from other records.

---

## Non-Functional Requirements

Non-functional requirements are the **constraints and quality attributes** that define **how the system should perform**, rather than what functions it should provide. They apply to the system as a whole, rather than to individual features or services, and include aspects like performance, usability, reliability, security, and compliance with standards. These requirements often specify timing constraints, development process standards, system capacity, security measures (e.g., protection against SQL injection), failure rates, programming languages, tools to be used, and organizational policies the system must follow.

Non-functional requirements are often **more critical** than individual functional requirements. While users may find workarounds if a function does not fully meet their needs, failing to meet non-functional requirements can make the entire system unusable.

**Examples:**
- The system should load within 3 seconds.    
- It should be available 24/7 with 99.9% uptime.    
- All user data must be stored securely and encrypted.    

Non-functional requirements are essential for ensuring a good **user experience** and system **performance**, helping to evaluate how well the system meets user expectations beyond just its core functions.
