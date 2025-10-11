---
class: cse
title: 02 Give the transmission media and topologies recommended for Fiber Channel (FC).
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
Note: see the exam kit answer of this question
---
# Transmission Media and Topologies for Fiber Channel (FC)

Fiber Channel (FC) is a high-speed network technology mainly used for storage area networks (SANs). It provides fast, reliable, and low-latency communication between servers and storage devices. The choice of transmission media and topology impacts the speed, reliability, and scalability of the network.

---

**Transmission Media:**  
The primary medium for FC is **optical fiber**, which supports very high speeds, is immune to electromagnetic interference, and allows long-distance communication up to several kilometers. **Copper cables**, such as twisted pair or shielded twisted pair, are also used for short-distance connections, offering a cost-effective solution but with limited speed and range compared to fiber.

---

**Recommended Topologies:**

1. **Point-to-Point Topology:** A direct connection between two devices. It is simple and fast but not suitable for large networks due to scalability limits.    
2. **Arbitrated Loop Topology (FC-AL):** Devices are connected in a ring structure, allowing only one device to transmit at a time. This topology is cost-effective for small to medium SANs.    
3. **Switched Fabric Topology (FC-SW):** Devices are connected through FC switches, enabling multiple simultaneous communications. It is highly scalable, efficient, and ideal for large, high-performance storage networks.