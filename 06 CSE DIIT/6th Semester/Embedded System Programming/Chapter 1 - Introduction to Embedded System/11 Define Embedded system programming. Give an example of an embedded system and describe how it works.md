---
class: cse
title: 02 Define Embedded system programming. Give an example of an embedded system and describe how it works
course:
  - Embedded System Programming
chapter:
  - chapter 1 - Introduction to Embedded System
semester: 6th
date: 2025-07-28
status: pending 🛑
tags:
  - ESP/Ch1
---

## Embedded system programming

**Embedded system programming** is the process of writing software code that runs on an **embedded system** — a combination of hardware and software designed to perform a specific task within a larger system.

This type of programming is focused on:
- Controlling hardware devices (like sensors, actuators, displays)    
- Managing real-time data processing    
- Ensuring performance under limited memory, power, and processing speed    

The code is usually written in **C, C++, or Assembly**, and stored in the system’s **ROM or flash memory**. It interacts closely with the hardware to carry out predefined tasks automatically, reliably, and often in real-time.

---

## Example of an embedded system 

Example: **Digital Blood Pressure Monitor**

An embedded system in a **digital blood pressure monitor** demonstrates how such programming works in real life.

### Working Process

1. **Microcontroller**: The central unit contains an embedded program that controls all operations.    
2. **Input Sensors**: Pressure sensors detect the pressure in the cuff during inflation and deflation.    
3. **Processing**:    
    - The embedded software calculates systolic and diastolic values using sensor data.        
    - It applies algorithms to remove noise and measure accurate readings.        
4. **Display Output**: Results are shown on an LCD screen.    
5. **User Interface**: Buttons allow the user to start, reset, or choose memory options.    
6. **Power Management**: The embedded system controls battery usage efficiently.
