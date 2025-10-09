---
class: cse
title: 15 With a configuration of TCP/IP show the operation of the following
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-07-08
status: pending 🛑
importance: ⭐⭐⭐⭐⭐
Note: " Figures are in exam-kit question no. 26"
tags:
  - board_2019
  - board_2021
topic: Topic 03 - TCP/IP Protocol Suite
---
**With a configuration of TCP/IP show the operation of the following -**

   1. **action to sender**  
   2. **action to router**  
   3. **action receiver**

---

## Operation of TCP/IP for the Given Actions

**1. Action to Sender:**  

```bash
Action to Sender
Application
    ⬇️
Data
    ⬇️
TCP
    ⬇️
IP
    ⬇️
LLC
    ⬇️
MAC
    ⬇️
Physical
```

- At the sender’s side, the process begins at the Application layer, where the data (such as a web request or file) is generated. 
- This data is then passed to the Transport layer (usually TCP), which breaks the data into smaller segments, adds port numbers to identify the sending and receiving applications, **sequence numbers** to keep track of order, and a **checksum** to detect errors during transmission to ensure reliable delivery. 
- Next, the Internet layer adds the source and destination IP addresses, forming packets that can be routed across networks. 
- Finally, the Network Access layer takes these packets and converts them into frames suitable for the physical medium (like Ethernet or Wi-Fi) and sends the frames out over the physical network.

**2. Action to Router:**  

```bash
Action to Router
Physical
    ⬇️
MAC
    ⬇️
LLC
    ⬇️
IP
    ⬇️
Check destination & routing
    ⬇️
LLC
    ⬇️
MAC
    ⬇️
Physical
```

- When the data reaches a router, the Network Access layer on the router receives the frame and extracts the packet from it. 
- The Internet layer then reads the destination IP address of the packet and consults the router’s routing table to determine the best next hop toward the destination.
- The router then encapsulates the packet into a new frame appropriate for the next network segment and forwards it along. 
- This process of receiving, examining, and forwarding repeats at every router until the packet arrives at the receiver’s network.

**3. Action to Receiver:**  

```bash
Action to Receiver
Physical
    ⬇️
MAC
    ⬇️
LLC
    ⬇️
IP
    ⬇️
TCP
    ⬇️
Data
    ⬇️
Application
```

- At the receiver’s end, the Network Access layer receives the incoming frame and extracts the packet. 
- The Internet layer verifies that the packet’s destination IP address matches its own address. 
- The Transport layer (TCP) then performs error checking to ensure data integrity and uses acknowledgments to confirm receipt. If any segments are missing or out of order, TCP requests retransmission or reorders them properly. 
- Finally, the data is passed up to the Application layer, where it is processed for use, such as displaying a webpage or opening a file.