---
class: cse
title: 02 Differentiate between API and system call.
course:
  - Embedded System Programming
chapter:
  - "ch3: Active X"
semester: 6th
date: 2025-09-05
status: pending 🛑
importance: ⭐⭐⭐
tags:
  - board_2022
topic: Set 01
---

### Definition of API

An **Application Programming Interface (API)** is a high-level interface that allows different applications or software components to communicate. It provides predefined functions and protocols, making software development easier without exposing internal system details.

### Definition of System Call

A **System Call** is a low-level mechanism that allows a program to directly request services from the operating system kernel, such as file handling, memory management, and process control.

---

### Difference between API and System Call

> NOTE: _see exam kit page no. 317 different table_

|Aspect|API (Application Programming Interface)|System Call|
|---|---|---|
|**Meaning**|Interface between applications or between application and service.|Interface between user program and OS kernel.|
|**Level of Operation**|High-level (user/application level).|Low-level (kernel/OS level).|
|**Abstraction**|Provides abstraction from system and hardware details.|Provides minimal abstraction, directly exposes OS services.|
|**Ease of Use**|Easier to use; designed for developers (functions, libraries).|More complex; requires understanding of OS mechanisms.|
|**Portability**|Portable across platforms if API exists (e.g., Java API, Web API).|Platform dependent (system calls vary between OS).|
|**Examples**|Java API, Google Maps API, REST API.|`open()`, `read()`, `write()`, `fork()` in Unix/Linux.|