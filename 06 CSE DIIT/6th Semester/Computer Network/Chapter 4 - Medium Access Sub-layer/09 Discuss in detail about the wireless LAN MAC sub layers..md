---
class: cse
title: 09 Discuss in detail about the wireless LAN MAC sub layers.
course:
  - Computer Network
chapter:
  - Chapter 4 - Medium Access Sub-layer
semester: 6th
date: 2025-09-06
status: pending 🛑
tags:
  - CN/Ch4
---

## Wireless LAN MAC Sublayers

The **MAC (Medium Access Control) sublayer** in a wireless LAN is responsible for **controlling access to the shared wireless medium**. Due to the nature of wireless communication, it handles challenges like **collisions, hidden nodes, and interference**. The MAC sublayer is divided into **two main sublayers**:

1. **Distributed Coordination Function (DCF)** – DCF is a **contention-based sublayer** where stations compete for access to the medium. It uses **CSMA/CA (Carrier Sense Multiple Access with Collision Avoidance)** to avoid collisions. Before transmitting, a station listens to the medium. If the medium is busy, it waits for a **random backoff period** before trying again. DCF can also use **RTS (Request to Send) and CTS (Clear to Send)** signals to prevent collisions caused by hidden nodes. This ensures fair access to all stations and improves reliability in environments with multiple devices.

---

2. **Point Coordination Function (PCF)** – PCF is an **optional, centralized sublayer** designed to provide **collision-free access**. The **access point acts as a point coordinator**, polling stations in a specific order and granting permission to transmit. This polling mechanism is useful for **time-sensitive traffic**, such as voice or video, where predictable transmission times are required. PCF operates on top of DCF and allows the network to provide **better quality of service**.

