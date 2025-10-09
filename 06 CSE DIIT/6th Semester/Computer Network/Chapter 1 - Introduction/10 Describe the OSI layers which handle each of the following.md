---
class: cse
title: 10 Describe the OSI layers which handle each of the following
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-07-08
status: done ✅
tags:
  - CN/Ch1/board_2020
---

**Describe the OSI layers which handle each of the following -** 

   1. **Breaking the transmitted bit stream into frame**  
   2. **Determine the which router through the subnet is used**

---

### 1. Breaking the transmitted bit stream into frames

This task is performed by the **Data Link Layer** (Layer 2) of the OSI model.  
The Data Link Layer is responsible for **framing**, which means converting the continuous stream of bits received from the Physical Layer into structured data units called **frames**. These frames contain not only the actual data but also **control information**, such as:

- **Start and end of frame markers**    
- **MAC (Media Access Control) addresses**    
- **Error detection codes** (e.g., CRC – Cyclic Redundancy Check)    

Framing allows the receiving device to clearly identify where each message starts and ends. This layer also ensures **error detection**, **flow control**, and **medium access control** in local area networks (LANs). It plays a crucial role in reliable communication over a single physical link between two directly connected nodes.

---

### 2. Determining which router through the subnet is used

This function is managed by the **Network Layer** (Layer 3) of the OSI model.  
The primary responsibility of the Network Layer is to ensure **end-to-end delivery of packets** across different networks. It uses **logical addressing** (such as IP addresses) to identify devices across networks.

When a packet is to be sent from the source to the destination, and they are on different networks, the Network Layer determines the **most efficient path** through the subnet by:

- **Analyzing routing tables**    
- **Using routing protocols** (e.g., RIP, OSPF, BGP)    
- **Selecting the next router (hop)** based on metrics like hop count, delay, bandwidth, etc.    

This process is known as **routing**. The chosen router forwards the packet closer to the destination, and each router along the path repeats this process until the packet reaches its final destination.


- 🥤 (pomodoro::BREAK) (duration:: 5m) (begin:: 2025-08-04 08:55) - (end:: 2025-08-04 09:00)