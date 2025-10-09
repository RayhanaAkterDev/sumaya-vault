---
class: cse
title: 19 What do you mean by transmission. What can be the different direction of transmission
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-08-05
status: done ✅
tags:
  - CN/Ch1/board_2017
---

## Transmission

**Transmission in computer networks** refers to the process of sending and receiving data such as text, audio, or video between devices through a communication medium like cables, fiber optics, or radio waves. It involves converting digital data into suitable signals—electrical, optical, or electromagnetic—that can travel across the chosen medium and be interpreted correctly at the destination. Transmission is a core function of networking, as it ensures effective communication between devices, networks, and systems, making data exchange possible in both local and global contexts.

### Directions of Transmission

The **direction of data transmission** determines how data flows between sender and receiver. There are **three standard transmission directions**:

#### Simplex Transmission

Simplex transmission is a **unidirectional** method of communication in which **data flows in only one direction**, i.e., from the sender to the receiver. The receiver **cannot send any data back** to the sender. Best suited for devices with a fixed sender/receiver role. **Example:** 
- Keyboard input to CPU
- Radio and TV broadcasting

#### Half-Duplex Transmission 

Half-duplex transmission is a **bidirectional** communication method, but data can flow in **only one direction at a time**. Requires control mechanisms to avoid collision. The sender and receiver can both transmit data, but **not simultaneously**. More efficient than simplex as both devices can communicate, though not at the same time. **Example:**
- Walkie-talkies
- Traditional police radio systems

#### Full-Duplex Transmission 

Full-duplex transmission allows **simultaneous two-way communication**. Both the sender and the receiver can send and receive data at the **same time**. Most efficient among the three modes. Requires dedicated channels for both directions or intelligent channel separation. Ideal for real-time applications requiring instant interaction. **Example:**
- Telephone systems
- Modern online video conferencing