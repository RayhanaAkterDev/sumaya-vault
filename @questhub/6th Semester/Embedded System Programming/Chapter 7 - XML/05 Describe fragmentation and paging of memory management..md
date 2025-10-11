---
class: cse
title: 05 Describe fragmentation and paging of memory management.
course:
  - Embedded System Programming
chapter:
  - "ch7: XML"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2021
---
# Fragmentation and Paging in Memory Management

In memory management, efficient utilization of limited memory is crucial, especially in embedded systems and operating systems. Two important concepts that affect memory usage are **fragmentation** and **paging**.

**Fragmentation** occurs when memory is not used efficiently, leaving small unused blocks that cannot satisfy new memory requests. Fragmentation reduces the effective available memory and can cause allocation failures or performance issues if not managed properly. There are two main types:

1. **External Fragmentation** – Free memory is split into small non-contiguous blocks. Even if the total free memory is enough, a large process cannot be allocated because the memory is fragmented.    
2. **Internal Fragmentation** – Allocated memory blocks may be slightly larger than requested, leaving unused space inside the block, wasting memory.

---

**Paging** is a memory management technique that divides physical memory and processes into fixed-size blocks called **pages** (for processes) and **frames** (for memory). The OS maps pages to frames, allowing non-contiguous allocation.

Key points about paging:

1. Eliminates external fragmentation since pages can be placed anywhere in memory.    
2. Makes memory allocation flexible and efficient.    
3. Requires a **page table** to track which page is stored in which frame.    

**Example / Use Case**  
If a process requires 6 KB of memory and memory frames are 1 KB each, the process is divided into six pages that can occupy any available frames in memory. Paging ensures that memory is used efficiently without leaving unusable gaps caused by external fragmentation.