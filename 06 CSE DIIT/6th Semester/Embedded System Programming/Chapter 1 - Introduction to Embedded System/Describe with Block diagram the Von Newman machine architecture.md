---
class: cse
title: Describe with Block diagram the Von Newman machine architecture
course:
  - Embedded System Programming
chapter:
  - "ch1: Introduction to Embedded System"
semester: 6th
date: 2025-09-20
status: pending ⏳
importance: ⭐⭐⭐⭐⭐
tags:
  - board_2021
topic: Set 01
---
## Von Neumann Machine Architecture

The Von Neumann architecture, proposed by John von Neumann in 1945, is based on the **stored-program concept**, where both instructions and data are stored in the same memory. The CPU executes instructions sequentially through the **fetch–decode–execute cycle**, with the control unit coordinating all computer operations. This design is simple, flexible, and cost-effective, forming the foundation of all modern general-purpose computers.

### Main Components of Von Neumann Architecture

![[Pasted image 20250920184810.png]]

- **Central Processing Unit (CPU)**: It is called the "brain" of the computer. Performs all processing tasks, calculations, and decision-making. Contains the Control Unit (CU), Arithmetic Logic Unit (ALU), and registers.
	- **Control Unit (CU)**: It directs the flow of data between CPU, memory, and input/output devices. Fetches instructions from memory, decodes them, and controls execution.
	- **Arithmetic Logic Unit (ALU)**: Handles all arithmetic operations (addition, subtraction, multiplication, division). Performs logical operations (AND, OR, NOT, comparisons).        
	- **Registers**: They are small, high-speed storage inside the CPU. Temporarily hold data, instructions, and intermediate results during processing.        
- **Memory (Main Memory / RAM)**: The memory stores both data and program instructions. Organized in sequential addresses for quick access. Acts as the working storage area for the CPU.
- **Input/output Devices (I/O)**:    
    - Input devices (keyboard, mouse, sensors) allow users to send data and instructions.        
    - Output devices (monitor, printer) display or deliver processed results.        
- **System Bus**: The system bus is a communication pathway connecting CPU, memory, and I/O. Consists of three types of buses:
	1. **Data Bus** – transfers actual data.
	2. **Address Bus** – carries memory or device addresses.
	3. **Control Bus** – sends control signals like read, write, or clock.

---

## **Operation Cycle (Fetch–Decode–Execute Cycle)**

1. **Fetch**: The **Control Unit (CU)** uses the **Program Counter (PC)** to locate the next instruction in memory. The instruction is fetched from memory and placed into the **Instruction Register (IR)**.
2. **Decode**: The CU interprets (decodes) the fetched instruction. It determines **what operation** is required and **which operands** (data/addresses) are involved.
3. **Execute**: The instruction is carried out. The **ALU** performs arithmetic or logical operations, or the CU coordinates data transfer between CPU, memory, and I/O.
4. **Store**: The result of the execution is stored in a **register** or written back to **main memory** if needed.
5. **Repeat**: The **Program Counter** is updated to point to the next instruction, and the cycle repeats continuously.

---

##  General Machine Structure

It is the basic model of a computer system which describes the fundamental layout of a computer system and how the computer works. It consists of **input**, **memory**, **CPU (with ALU and CU)**, and **output**, all connected by a **system bus**. Both data and instructions are stored in the same memory, and the CPU processes them step by step using the fetch–decode–execute cycle.

![[621-general-machine-structure 1.png]]