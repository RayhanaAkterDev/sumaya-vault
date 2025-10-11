---
class: cse
title: 03 What is SONET and SDH? Which devices are used in SONET transmission?
course:
  - Software Engineering
chapter:
  - Chapter 6 - Optical Fiber Network
semester: 6th
date: 2025-09-11
status: pending 🛑
importance: ⭐⭐
tags:
  - board_2018
  - board_2020
  - board_2022
---
# SONET and SDH

**SONET (Synchronous Optical Network)** is a North American standard for transmitting large volumes of digital data over optical fiber in a synchronized manner. It allows the **multiplexing of multiple lower-rate digital signals** into high-speed optical signals while providing features like error detection, network management, and fast fault recovery. SONET supports high-speed communication (from OC-1 at 51.84 Mbps to OC-768 and beyond) and is widely used in backbone and metropolitan area networks.

**SDH (Synchronous Digital Hierarchy)** is the international equivalent of SONET, standardized by the ITU-T. It provides **high-speed, reliable, and scalable optical transport** for voice, data, and video signals. SDH is interoperable with SONET but follows slightly different frame structures and naming conventions. Both SONET and SDH enable efficient multiplexing, synchronous transmission, and easy network management for long-distance communication.

---

# Devices Used in SONET Transmission

1. **Terminal Multiplexer (TM):**  
    A TM combines multiple lower-speed digital signals (like DS-1 or DS-3) into a SONET optical signal. It ensures that data streams from various sources are synchronized and transmitted as a single high-speed signal. This device is typically used at the entry and exit points of the SONET network.
    
2. **Add-Drop Multiplexer (ADM):**  
    The ADM allows specific channels or signals to be added to or removed from a SONET line **without disturbing other channels**. This capability enables efficient network management and local access to high-speed lines while maintaining continuous end-to-end transport.
    
3. **Regenerator:**  
    Regenerators are used in long-distance SONET links to **amplify, reshape, and retime optical signals**. They compensate for signal attenuation and distortion over long fiber spans, ensuring that the transmitted data maintains integrity and synchronization.
    
4. **Digital Cross-Connect (DXC):**  
    DXCs are intermediate devices used to **switch SONET channels** between different paths in the network. They provide flexibility in routing, allow traffic management, and support protection mechanisms in case of link or device failures.
    
5. **Optical Line Terminal (OLT) / Optical Network Unit (ONU):**  
    In SONET-based access networks, OLTs interface the backbone network to local network devices, while ONUs serve as endpoints at customer premises. They handle **signal conversion between optical and electrical formats** and ensure proper synchronization with the SONET backbone.