---
class: cse
title: 03 Explain the ATM layers with their functions.
course:
  - Computer Network
chapter:
  - Chapter 3 - ATM Networks
semester: 6th
date: 2025-09-05
status: pending 🛑
tags:
  - board_2018
  - board_2021
---

### **ATM Layers and Their Functions**

ATM (Asynchronous Transfer Mode) is a **high-speed networking technology** that transmits data in small, fixed-size cells of 53 bytes. The ATM architecture is **layered**, similar to the OSI model, providing modularity and clear separation of responsibilities. The main layers of ATM are the **Physical Layer, ATM Layer, ATM Adaptation Layer (AAL), and Higher/Application Layer**.

1. **Physical Layer**  
    The Physical Layer is responsible for the **transmission of ATM cells over the physical medium**, such as fiber optics or copper cables. It handles bit-level functions such as encoding, synchronization, and error detection, ensuring that the sequence of ATM cells is delivered correctly to the next layer. This layer defines the electrical, optical, and mechanical characteristics of the network interface.
    
2. **ATM Layer**  
    The ATM Layer manages **cell-based operations** and ensures **reliable transport of cells** between end systems. Its key functions include cell multiplexing and demultiplexing, addressing, routing, and switching. The ATM layer focuses on the movement of cells without concerning itself with the content. It also handles cell-level error detection and supports both connection-oriented and connectionless services.
    
3. **ATM Adaptation Layer (AAL)**  
    The ATM Adaptation Layer adapts **higher-layer user data** into 48-byte payloads suitable for ATM cells. It provides services such as segmentation and reassembly, timing, error correction, and flow control. Different types of AAL exist to support different traffic types:
    
    - **AAL1**: Used for **constant bit rate (CBR)** services like voice and circuit emulation; provides timing and error recovery.        
    - **AAL2**: Supports **variable bit rate (VBR)** services such as compressed voice or multimedia; allows multiple low-speed streams over one ATM connection.        
    - **AAL3/4**: Designed for connection-oriented and connectionless data services; provides error detection and segmentation/reassembly.        
    - **AAL5**: Simplified AAL for **data transfer**, commonly used in IP over ATM; provides minimal overhead, end-to-end error detection, and segmentation/reassembly.

4. **Higher Layer / Application Layer**  
    The Higher Layer, or Application Layer, represents **user applications and services** that use the ATM network, such as voice, video, multimedia, and general data applications. It does not deal with cell transport directly but relies on lower layers for delivery. Key functions include:
    
    - **Service Utilization**: Applications access network services via AAL.        
    - **Traffic Type Definition**: Determines whether traffic is CBR, VBR, or UBR, guiding the choice of AAL.        
    - **End-to-End Communication**: Ensures that application data is delivered correctly, in order, and with the required timing, relying on lower layers for transport, segmentation, and error handling.