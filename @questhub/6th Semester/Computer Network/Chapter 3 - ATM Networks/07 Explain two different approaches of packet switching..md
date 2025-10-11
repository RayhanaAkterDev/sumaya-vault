---
class: cse
title: 07 Explain two different approaches of packet switching.
course:
  - Computer Network
chapter:
  - Chapter 3 - ATM Networks
semester: 6th
date: 2025-09-05
status: pending 🛑
tags:
  - board_2018
  - board_2020
  - board_2022
---

 ## Two Approaches of Packet Switching

Packet switching can be implemented using two main approaches: **Datagram Switching** and **Virtual Circuit Switching**. Both approaches allow data to be transmitted efficiently in a shared network, but they handle packet routing differently.

1. **Datagram Switching:**  
    In datagram switching, each packet is treated independently and carries the full destination address. Packets may take different routes through the network depending on traffic and availability. Since the packets can arrive out of order, the receiving end reassembles them to reconstruct the original message. This approach is flexible, efficient for bursty traffic, and does not require dedicated resources. However, it may cause variable delays and requires extra processing to reorder packets.  
    _Example:_ The Internet uses datagram switching.
    
2. **Virtual Circuit Switching:**  
    Virtual circuit switching establishes a logical path, or virtual circuit, between the sender and receiver before any packets are transmitted. All packets follow this predetermined path and arrive in the correct sequence. This method ensures predictable performance, easier error detection, and orderly delivery. However, it requires setup time and reserves resources along the path, which can reduce flexibility.  
    _Example:_ X.25 networks use virtual circuit switching.
