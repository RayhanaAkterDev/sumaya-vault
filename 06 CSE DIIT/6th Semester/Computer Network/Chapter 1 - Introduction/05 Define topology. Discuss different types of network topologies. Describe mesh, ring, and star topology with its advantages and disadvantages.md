---
class: cse
title: 05 Define topology. Discuss different types of network topologies. Describe mesh, ring, and star topology with its advantages and disadvantages
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-07-08
status: done ✅
tags:
  - CN/Ch1/board_2019
---

## Definition of Topology

Network topology refers to the structure of a network. Basically, refers to the physical or logical arrangement of computers, cables, switches, and other devices in a network. 

In simple words, **Topology** is the way in which computers, devices, and cables are arranged and connected in a network. It defines the structure of the network and how data flows between the devices. Topology includes two main aspects:

1. **Physical topology**: This topology emphasizes the physical layout of the connected devices and nodes
2. **Logical topology**: It focuses on the pattern of the data transfer between network nodes.

---

## ✅ **Types of Network Topologies (Based on Layout/Structure):**

> 1. **Bus Topology**: All devices are connected to a **single central cable** (called the bus). Data travels in both directions along this cable, and each device receives the data meant for it.	
>	- Simple and cost-effective for small networks    
>	- Requires less cable compared to others
>	- Terminators are needed at both ends of the bus    
>	- Performance degrades as more devices are added    
>	- One cable failure can bring down the entire network

> 2. **Star Topology**: All devices are connected to a **central hub or switch**. The hub acts as a controller, and data passes through it to reach other devices.
>	- Easy to install, configure, and manage
>	- Centralized control simplifies troubleshooting    
>	- Failure of a single node does not affect others    
>	- Entire network depends on the central hub’s functioning    
>	- Requires more cable than bus topology

> 3. **Ring Topology**: Devices are connected in a **circular loop**, where each device has exactly two neighbors. Data travels in one direction around the ring until it reaches the destination.
>	- Each device acts as a repeater to pass data forward
>	- Equal access for all devices (no data collision)    
>	- Performance remains stable under load    
>	- A break in the ring can disrupt communication    
>	- Dual ring (bidirectional) can be used for fault tolerance

> 4. **Mesh Topology**: Each device is connected **directly to every other device** in the network. It provides high reliability and redundancy but is expensive to implement.
>	- Offers high fault tolerance and reliability    
>	- Supports continuous communication even if one path fails    
>	- Full mesh and partial mesh variations available    
>	- Complex to design and expensive to implement    
>	- Requires more cabling and configuration

> 5. **Tree Topology**: A **hierarchical structure** that combines characteristics of both **star** and **bus** topologies. It starts with a root node and branches out like a tree.
>	- Ideal for large networks with a layered approach    
>	- Easier network expansion through branches    
>	- Failure of a main cable affects the entire branch    
>	- More structured and organized than pure star or bus    
>	- Easier for network segmentation and control

> 6. **Hybrid Topology**: A combination of **two or more different topologies**. It is flexible and scalable, commonly used in large organizations.
>	- Highly scalable and flexible in design    
>	- Can adapt to various use cases and network sizes    
>	- More resilient to faults compared to basic topologies    
>	- Complex to design and manage   
>	- Common in enterprise networks with multiple departments
 