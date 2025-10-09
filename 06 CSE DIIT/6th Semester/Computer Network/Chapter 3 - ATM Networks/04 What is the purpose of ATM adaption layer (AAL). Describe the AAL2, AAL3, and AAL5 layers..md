---
class: cse
title: 04 What is the purpose of ATM adaption layer (AAL). Describe the AAL2, AAL3, and AAL5 layers.
course:
  - Computer Network
chapter:
  - Chapter 3 - ATM Networks
semester: 6th
date: 2025-09-05
status: pending 🛑
tags:
  - board_2019
---

## ATM Adaptation Layer (AAL) – Purpose and Types

### Purpose of ATM Adaptation Layer (AAL)

The **ATM Adaptation Layer (AAL)** is a sublayer in the ATM (Asynchronous Transfer Mode) protocol stack that sits between the **ATM layer** and the **higher-layer applications**. Its main purpose is to adapt and convert different types of user traffic—such as voice, video, or data—into **fixed-size ATM cells (53 bytes)** for transmission over the ATM network. AAL ensures **segmentation and reassembly**, handles **timing and error control**, and provides **service-specific functions** required by higher-layer protocols.

---

### Types of ATM Adaptation Layers


> The **ATM Adaptation Layer (AAL)** is a sublayer in the ATM protocol stack that sits between the ATM layer and higher-layer applications. Its main purpose is to adapt different types of user traffic—such as voice, video, or data—into **fixed-size ATM cells** for transmission over the ATM network. The AAL handles **segmentation and reassembly**, provides **error detection**, and ensures that timing-sensitive data is delivered correctly, allowing multiple types of traffic to coexist efficiently.

> **AAL2** is designed for **real-time, low-latency applications** like voice and interactive multimedia. It supports **variable bit rate (VBR) traffic** and short packets, enabling multiple users to share the same ATM connection efficiently while ensuring timely delivery.

> **AAL3/4** is used for **connection-oriented or connectionless data transfer** with error detection and control. It segments messages into ATM cells and provides a per-cell header for identification and sequencing. While reliable, its per-cell headers introduce higher overhead, making it less efficient than newer AAL types.

> **AAL5** is a simplified and widely used version of AAL3. It provides **connection-oriented data transfer** with minimal overhead by adding a **trailer at the end of the message** for error checking and message delineation instead of per-cell headers. AAL5 is efficient and commonly used for applications like IP over ATM and other modern data communications where reliability and simplicity are important.