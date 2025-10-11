---
class: cse
title: 14 What is Input Injection in API?
course:
  - Embedded System Programming
chapter:
  - "ch3: Active X"
semester: 6th
date: 2025-09-05
status: pending 🛑
tags:
  - ESP/Ch3
---

### Definition of Input Injection

**Input Injection** in the context of APIs is a type of security vulnerability where an attacker sends **malicious or unexpected data** as input to an API, aiming to manipulate the API’s behavior, gain unauthorized access, or compromise the system. It occurs when the API does not properly validate or sanitize input before processing it.

Input injection can affect databases, command execution, or even other connected systems. If unchecked, it can lead to serious consequences such as data breaches, unauthorized actions, or system crashes.

---

### Example

1. **SQL Injection via API**: An attacker sends a specially crafted input to an API endpoint that queries a database. If the API does not validate the input, the database query may execute malicious commands, exposing sensitive data.
    
2. **Command Injection**: An attacker sends input that is interpreted as a system command by the API. This can allow them to execute commands on the server.
