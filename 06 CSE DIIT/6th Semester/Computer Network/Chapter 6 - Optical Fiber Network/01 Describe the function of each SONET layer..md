---
class: cse
title:
course:
  - Software Engineering
chapter:
  - Chapter 6 - Optical Fiber Network
semester: 6th
date: 2025-09-11
status: pending 🛑
importance: ⭐⭐⭐⭐
tags:
  - board_2021
---
# Functions of Each SONET Layer

**Introduction:**  
**SONET (Synchronous Optical Network)** is a standardized protocol for transferring multiple digital bit streams over optical fiber. Its layered architecture ensures efficient, reliable, and standardized communication. SONET consists of three main layers: **Physical Layer, Section Layer, and Line Layer**.

---

## 1. Physical Layer

The Physical Layer is responsible for the actual transmission and reception of raw bit streams over optical fiber. It ensures that the signal is correctly transmitted, received, and synchronized between network devices. This layer handles optical or electrical interfaces, converts signals between electrical and optical forms, and maintains bit timing.

**Example:**  
If a SONET device transmits at OC-3 (155 Mbps), the Physical Layer ensures the light pulses carrying bits are correctly sent and detected on the fiber.

---

## 2. Section Layer

The Section Layer manages the communication between two adjacent network elements. It ensures the integrity and correct sequencing of data as it travels from one device to another. The Section Layer monitors errors, maintains frame alignment, and provides the mechanisms to detect and report transmission faults within a single section of the network.

**Example:**  
When data passes between two SONET switches, the Section Layer checks for bit errors and maintains proper alignment of frames.

---

## 3. Line Layer

The Line Layer provides end-to-end transport of payloads across multiple sections. It is responsible for multiplexing lower-level signals into higher-order signals, monitoring line performance, and detecting and correcting errors along the line. This layer ensures that data is transmitted reliably from the source to the destination across the network.

**Example:**  
When multiple STS-1 signals are combined into an STS-3c signal, the Line Layer ensures that each lower-level signal reaches the destination correctly without loss or misalignment.