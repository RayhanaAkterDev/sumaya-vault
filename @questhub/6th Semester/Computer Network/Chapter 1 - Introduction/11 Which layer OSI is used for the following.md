---
class: cse
title: 11 Which layer OSI is used for the following
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-07-08
status: done ✅
importance: ⭐⭐⭐⭐⭐
tags:
  - board_2021
topic: Topic 02 - Reference Models (OSI and TCP/IP)
---

**Which layer OSI is used for the following -**  

   1. **To route packets**  
   2. **To convert packet to frame**  
   3. **To detect and correct errors**  
   4. **To run services like DNS, FTP, TELNET, etc.**

---

## 1. To route packets

This function is handled by the **Network Layer (Layer 3)** of the OSI model. The main responsibility of this layer is to determine the **best path** for data packets to reach their destination across multiple networks. It uses **logical addressing** (such as IP addresses) to identify devices on different networks. The Network Layer uses **routing algorithms** and protocols like RIP, OSPF, or BGP to make forwarding decisions. It ensures **packet delivery** even when the source and destination are not on the same local network by selecting appropriate routers along the path.

---

## 2. To convert packet to frame

The task of converting a packet into a frame is performed by the **Data Link Layer (Layer 2)**. This layer receives **network-layer packets** and encapsulates them into **frames** by adding headers and trailers containing **MAC (physical) addresses**, **error detection codes**, and **control information**. These frames are then passed to the Physical Layer for transmission over the physical medium. This conversion ensures that the data can be transmitted correctly over the local physical network (e.g., LAN or WAN link) and properly interpreted at the receiving end.

---

## 3. To detect and correct errors

The responsibility of error detection and correction is shared between the **Data Link Layer (Layer 2)** and the **Transport Layer (Layer 4)**. 

At the Data Link Layer, errors that occur in frames during transmission over a local link are detected using techniques like parity checks, checksum, and Cyclic Redundancy Check (CRC). It may also request retransmission of corrupted frames through ARQ protocols. 

At the Transport Layer, end-to-end error detection and recovery are provided by protocols such as TCP, which retransmit lost or corrupted segments. Together, these layers ensure reliable and accurate data communication across the network.

---

## 4. To run services like DNS, FTP, TELNET, etc.

These services operate at the **Application Layer (Layer 7)** of the OSI model. It is the topmost layer that directly interacts with **end-user applications** and provides **network-based services**. Protocols like **DNS** (for domain name resolution), **FTP** (for file transfer), **TELNET** (for remote login), **SMTP**, and **HTTP** all function at this layer. The Application Layer ensures that appropriate communication is established between the application software on both the sender’s and receiver’s sides. It also handles authentication, privacy, and data formatting needed for successful service execution.
