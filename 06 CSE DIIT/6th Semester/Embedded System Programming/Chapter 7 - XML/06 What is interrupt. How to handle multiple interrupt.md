---
class: cse
title: 06 What is interrupt? How to handle multiple interrupt?
course:
  - Embedded System Programming
chapter:
  - "ch7: XML"
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2020
---
# Interrupt and Handling Multiple Interrupts

An **interrupt** is a signal sent by a hardware device or software to the processor, requesting immediate attention. When an interrupt occurs, the normal execution of a program is temporarily halted, and the processor jumps to a special routine called the **Interrupt Service Routine (ISR)** to handle the event. After completing the ISR, the processor resumes the previously suspended task. Interrupts allow systems to respond quickly to important events such as input from a keyboard, timer expiration, or data transfer from an I/O device.

**Handling Multiple Interrupts**: When multiple interrupts occur together or during the servicing of another interrupt, the system needs a strategy to manage them efficiently. The main approaches are:

1. **Interrupt Priority** – Each interrupt is assigned a priority level by hardware or software. If two interrupts occur at the same time, the higher-priority one is serviced first. This prevents critical events (like emergency shutdown signals) from being delayed by less important ones.

2. **Interrupt Nesting** – A higher-priority interrupt can interrupt the execution of a lower-priority ISR. The CPU saves the current ISR state, executes the higher-priority ISR, and then resumes the lower-priority one. This ensures urgent tasks are not delayed but increases system complexity.
   
3. **Polling** – In this method, the processor checks all devices or sources one by one in a predefined order to identify which interrupt occurred. Although simple to implement, polling is slower compared to priority-based handling because the CPU wastes time checking sources even if only one has triggered.
   
4. **Vectored Interrupts** – Instead of a common ISR, each interrupt has its own unique memory address pointing directly to its ISR. This reduces the time needed to identify and handle interrupts, making the response faster and more efficient.
   

**Example**  
In a microcontroller-based system, if a UART interrupt (data received) and a timer interrupt (timeout) occur together, the processor uses the priority scheme. If the UART interrupt has higher priority, it will be serviced first, while the timer interrupt will either wait (if priorities are strict) or resume later (if nesting is allowed).