---
class: cse
title: "07 \rWhich devices are used in SONET transmission?"
course:
  - Software Engineering
chapter:
  - Chapter 6 - Optical Fiber Network
semester: 6th
date: 2025-09-11
status: pending 🛑
importance:
tags:
  - CN/Ch6
---
# Devices Used in SONET Transmission

SONET (Synchronous Optical Network) is a standardized protocol for high-speed data transmission over optical fiber. To implement SONET networks efficiently, several devices are required to **combine, manage, transmit, and maintain the integrity of digital signals** across the network.

---

**1. Terminal Multiplexer (TM):**  
The Terminal Multiplexer combines multiple lower-speed digital signals, such as DS-1 or DS-3, into a single high-speed SONET signal for transmission. It ensures that data streams from different sources are synchronized and properly formatted for the SONET network. TMs are usually located at the network entry and exit points.

**2. Add-Drop Multiplexer (ADM):**  
The Add-Drop Multiplexer allows specific channels to be added to or removed from a SONET line without affecting other channels. This enables efficient local access to high-speed lines and provides flexibility in network management. ADMs are widely used in metropolitan area networks to connect local sites to long-distance SONET links.

**3. Regenerator:**  
Regenerators are used in long-distance SONET networks to maintain signal quality. They amplify, reshape, and retime optical signals, compensating for signal attenuation and distortion that occur over long fiber spans.

**4. Digital Cross-Connect (DXC):**  
Digital Cross-Connects are intermediate devices that provide switching of SONET channels. They enable traffic to be rerouted dynamically, support network management, and provide protection in case of link or device failures.

**5. Optical Line Terminal (OLT) / Optical Network Unit (ONU):**  
In access networks based on SONET, OLTs connect the backbone network to the local network devices, while ONUs serve as endpoints at customer premises. These devices handle signal conversion between optical and electrical formats and maintain synchronization with the SONET network.

---

**Example:**  
In a metropolitan area SONET network, multiple office locations send low-speed digital signals to a Terminal Multiplexer. The signals are then transmitted over fiber, with Add-Drop Multiplexers removing or inserting specific signals at intermediate sites. Regenerators maintain signal integrity over long distances, and Digital Cross-Connects manage routing and redundancy to ensure reliable delivery.