---
class: cse
title: 06 Write down two problems in 802.11 MAC sub layer protocol.
course:
  - Computer Network
chapter:
  - Chapter 4 - Medium Access Sub-layer
semester: 6th
date: 2025-09-06
status: pending 🛑
tags:
  - board_2020
---

### **Problems in 802.11 MAC Sublayer Protocol**

1. **Hidden Node Problem** – In wireless networks, some stations may be **out of range of each other** but still able to communicate with the same access point. If these hidden nodes transmit simultaneously, their signals collide at the access point, leading to data loss. The standard MAC protocol cannot always detect such nodes, which **increases the probability of collisions** and reduces network efficiency. Techniques like **RTS/CTS (Request to Send / Clear to Send)** are used to partially solve this problem, but they add extra overhead.

> **Hidden Node Problem** – In a wireless network, some stations may be **out of range of each other** but still able to communicate with the same access point. If two hidden nodes transmit at the same time, their signals collide at the access point, causing **data loss** and forcing retransmissions. The standard 802.11 MAC sublayer relies on carrier sensing, but it cannot detect nodes that are hidden from each other, making it difficult to avoid such collisions. This problem **reduces network efficiency** and increases delays, especially in dense wireless environments. Protocol mechanisms like **RTS/CTS (Request to Send / Clear to Send)** help reduce the impact, but they also add extra overhead, slightly lowering throughput.
    
2. **Exposed Node Problem** – A station may sense that a neighboring station is transmitting and **unnecessarily postpone its own transmission**, even though sending would not interfere. This occurs because the MAC protocol is conservative in avoiding collisions, leading to **underutilization of the available bandwidth** and lower overall throughput.

> **Exposed Node Problem** – The exposed node problem occurs when a station **senses that a neighboring station is transmitting** and unnecessarily defers its own transmission, even though sending would not actually cause a collision. This happens because the MAC protocol conservatively assumes that any detected transmission could interfere with its own, leading to **underutilization of the wireless medium**. As a result, available bandwidth is wasted, and the overall network throughput decreases. This problem is common in networks with multiple overlapping coverage areas, where stations are within range of one transmitter but not of the receiver.
    
3. **Collision in Wireless Medium** – Unlike wired networks, wireless signals can **attenuate, fade, or be interfered with by obstacles**. Even with carrier sensing, the MAC protocol cannot always perfectly avoid collisions, especially in congested environments. This results in **frequent retransmissions** and reduced efficiency.
    
4. **Limited Support for QoS (Quality of Service)** – The basic 802.11 MAC protocol provides equal access to all stations and does not prioritize **time-sensitive traffic** like voice or video. This can lead to **delays or jitter**, affecting performance for applications that require consistent bandwidth.