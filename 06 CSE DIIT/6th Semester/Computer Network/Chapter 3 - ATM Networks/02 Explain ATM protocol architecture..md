---
class: cse
title: 02 Explain ATM protocol architecture.
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

### **ATM Protocol Architecture**

ATM (Asynchronous Transfer Mode) is a **cell-based, high-speed networking technology** designed to support a wide range of services such as voice, video, and data over a unified network. The ATM protocol architecture defines how data is transmitted, routed, and adapted across the network, and it is structured into **layers** to ensure modularity, interoperability, and efficient transport.

#### **ATM Layers**

1. **Physical Layer** – Responsible for the actual transmission of ATM cells over the physical medium. It ensures bit-level synchronization and maintains the integrity of transmitted data.

2. **ATM Layer** – Manages cell-level operations such as switching, routing, and addressing. It ensures cells are delivered in the correct sequence to the correct destination.
   
3. **ATM Adaptation Layer (AAL)** – Adapts user data into ATM cells and reassembles them at the destination. It has different types: **AAL1** for constant bit rate, **AAL2** for variable bit rate, **AAL3/4** for connection-oriented/connectionless data, and **AAL5** for efficient data transfer.

4. **Higher Layer / Application Layer** – Represents user applications and services like voice, video, or data. It defines traffic types and timing requirements, relying on lower layers for transport.


---

**Key Features of ATM Protocol Architecture:**

- **Cell-Based Transmission**: Data is transmitted in fixed-size 53-byte cells, allowing efficient multiplexing of voice, video, and data.    
- **Connection-Oriented Service**: Virtual circuits (PVCs or SVCs) are established before data transfer to ensure reliable delivery.    
- **Quality of Service (QoS)**: Different AAL types support different traffic requirements, such as low latency for voice or guaranteed delivery for data.    
- **Scalability and Flexibility**: ATM can carry multiple types of services on the same network infrastructure.