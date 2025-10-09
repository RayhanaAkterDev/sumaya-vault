---
class: cse
title:
course: Embedded System Programming
chapter:
  - "ch5: Multithread, XSLT"
semester: 6th
date: 2025-09-13
status: pending 🛑
tags:
  - board_2021
  - board_2022
---
## Multithreading

**Multithreading** is a technique in which a single program is divided into multiple threads, allowing them to execute concurrently. Each thread runs independently but shares the same memory and resources of the parent process, enabling efficient communication and faster execution. Multithreading improves system responsiveness, as multiple tasks can be performed simultaneously without blocking the main program flow. It is widely used in embedded systems, operating systems, and real-time applications to manage multiple tasks efficiently.

**Example:** In an embedded robotic system, one thread can continuously read sensor data, another can control motor movements, and a third can manage communication with a control panel. By running these threads concurrently, the system remains responsive and can handle multiple tasks simultaneously.