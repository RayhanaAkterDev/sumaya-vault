---
class: cse
title: 17 Give an example of an embedded system and describe how it works.
course:
  - Embedded System Programming
chapter:
  - chapter 1 - Introduction to Embedded System
semester: 6th
date: 2025-08-04
status: pending 🛑
tags:
  - ESP/Ch1
---

## Example of an Embedded System and How It Works

**Example:** **Washing Machine Embedded System**

A washing machine uses an embedded system to automate the entire washing process. The system consists of a **microcontroller**, **memory**, **input sensors**, **output actuators**, and **firmware/software**.

**How it works:**

1. **Input Stage:** The user selects the washing program (e.g., normal, delicate, or quick wash) through a keypad, dial, or touchscreen. Input sensors measure parameters like water level, water temperature, detergent amount, and drum load.
    
2. **Processing Stage:** The **microcontroller** reads inputs from the sensors and user interface. Using the program instructions stored in **ROM/flash memory**, it determines the correct sequence of operations, timing, and power settings for washing, rinsing, and spinning cycles.
    
3. **Output Stage:** The microcontroller sends signals to **actuators** such as the motor, water inlet valve, heater, and drain pump. These actuators perform physical actions: filling water, heating water to the required temperature, rotating the drum, dispensing detergent, and draining water.
    
4. **Monitoring and Feedback:** The embedded system continuously monitors sensor readings to ensure the washing process is performed correctly. If any abnormality occurs, such as water overflow or incorrect temperature, the system adjusts operations or stops to prevent damage.
