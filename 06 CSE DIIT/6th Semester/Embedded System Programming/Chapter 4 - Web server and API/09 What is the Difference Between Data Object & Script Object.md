---
class: cse
title: 09 What is the Difference Between Data Object & Script Object?
course:
  - Embedded System Programming
chapter:
  - "ch4: Web server and API"
semester: 6th
date: 2025-09-06
status: pending 🛑
tags:
  - ESP/Ch4
---

### **Difference Between Data Object and Script Object**

|Aspect|Data Object|Script Object|
|---|---|---|
|**Definition**|Represents and manages data as a container of attributes and sometimes methods.|A programmable component that contains reusable scripts, functions, or procedures.|
|**Purpose**|Used to store, organize, and transfer structured data.|Used to define logic, automate tasks, and extend application functionality.|
|**Focus**|Focuses on **data representation** and information handling.|Focuses on **actions, events, and processing logic**.|
|**Content**|Contains attributes (fields/variables) and may include methods for data manipulation.|Contains scripts, functions, and procedures for handling events or operations.|
|**Behavior**|Generally passive; stores data and may have minimal methods to manipulate it.|Active; executes code, handles events, and performs tasks automatically.|
|**Reusability**|Can be reused wherever structured data is needed.|Can be reused wherever specific scripts or logic are required.|
|**Interaction**|Interacts with applications by passing or storing data.|Interacts with other objects, applications, or the environment through scripts.|
|**Dependency**|Often depends on the application or database to utilize the data.|Can operate independently or be embedded in applications for added functionality.|
|**Examples**|_Student Data Object_ with fields like `ID`, `Name`, `Course`.|_Form Validation Script Object_ with methods to check user input.|
|**Typical Use Cases**|Data transfer between modules, database interaction, storing application state.|Event handling, automation, dynamic behavior in web pages or applications.|