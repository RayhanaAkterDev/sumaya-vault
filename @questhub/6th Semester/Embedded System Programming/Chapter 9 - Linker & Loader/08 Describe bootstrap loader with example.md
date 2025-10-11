---
class: cse
title: 08 Describe bootstrap loader with example
course: Embedded System Programming
chapter:
  - "ch9: Linker & Loader"
semester: 6th
date: 2025-09-11
status: pending 🛑
importance: ⭐⭐
tags:
  - board_2020
  - board_2021
  - board_2022
topic: Set 05 & 06
---
### Bootstrap Loader

A **bootstrap loader** is a special type of loader that is responsible for **initiating the startup process of a computer system**. It is a small, essential program stored in **ROM (Read-Only Memory)** or firmware, and its primary function is to **load the operating system (OS) into main memory** when the computer is powered on or restarted. Since the main OS is stored on secondary storage (like a hard disk), the bootstrap loader provides the **first set of instructions** to start the system and transfer control to the operating system.

The bootstrap loader works in the following steps:

1. **Power-On or Reset:** When the computer is switched on, the CPU begins executing instructions from a fixed memory location in ROM, where the bootstrap loader resides.
    
2. **Hardware Initialization:** It performs **basic hardware checks** and initializes essential devices, such as memory and input/output controllers.
    
3. **Loading the OS:** It locates the **operating system kernel** on the secondary storage and loads it into main memory.
    
4. **Transfer Control:** After loading the OS, it transfers **control to the operating system**, which then takes over full management of the system.

**Example:**  
When you start a computer, the BIOS or UEFI contains the bootstrap loader. It checks the hardware, finds the bootable device, loads the operating system (like Windows or Linux) from the hard drive into memory, and starts execution.