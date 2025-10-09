---
class: cse
title: 16 Define unicasting, multicasting, and broadcasting network
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-07-08
status: done ✅
tags:
  - CN/Ch1/board_2022
  - CN/Ch1/board_2019
---

### **Unicasting**

Unicasting is a communication method where data is sent from one sender to one specific receiver. It is a one-to-one transmission, where each data packet is addressed to the unique IP address of the receiver. This method ensures that only the intended device receives the message. Unicasting is commonly used in regular internet activities like browsing websites or sending emails. However, if the same data needs to be sent to many users, unicasting requires sending separate copies, which can be inefficient.

---

### **Multicasting**

Multicasting is a one-to-many communication method where a sender transmits data to a specific group of receivers simultaneously. Instead of sending multiple copies, the sender sends a single stream to a multicast IP address, and only devices that have joined the multicast group receive the data. This approach conserves bandwidth and reduces network traffic, making it highly efficient for delivering data to multiple users. Protocols like IGMP (IPv4) or MLD (IPv6) manage group membership. Multicasting is commonly used in applications such as live video streaming, online gaming, IPTV, and real-time data feeds, where the same content needs to be delivered to many users at once.

---

### **Broadcasting**

Broadcasting is a one-to-all communication method where a sender transmits data to all devices within the same local network segment. The message is sent to a broadcast address (e.g., 255.255.255.255), and every device in the network processes the data. It is useful for tasks such as device discovery, ARP requests, or DHCP messages. However, because all devices receive the broadcast, excessive broadcasting can cause network congestion and slow down performance. Unlike multicasting, broadcasting does not support targeted delivery and is limited to local network communication.
