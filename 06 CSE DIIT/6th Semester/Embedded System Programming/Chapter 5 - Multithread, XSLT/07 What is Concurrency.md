---
class: cse
title: 07 What is Concurrency?
course: Embedded System Programming
chapter:
  - "ch5: Multithread, XSLT"
semester: 6th
date: 2025-09-13
status: pending 🛑
tags:
  - ESP/Ch5
---
## Concurrency

**Concurrency** is the ability of a system to manage and execute multiple tasks or processes in overlapping time periods, allowing them to make progress simultaneously. It enables programs to perform several operations at the same time, improving efficiency, responsiveness, and resource utilization. Even on a single processor, concurrency is achieved by interleaving task execution so that the CPU switches rapidly between tasks. On multi-core systems, tasks can run truly in parallel. Concurrency is widely used in embedded systems, operating systems, and real-time applications to optimize performance, reduce idle time, and handle multiple operations effectively.

**Example:** In a robotic system, one thread reads sensor data while another controls motors. Both tasks progress concurrently, enabling the robot to operate efficiently without waiting for one task to finish before starting the other.