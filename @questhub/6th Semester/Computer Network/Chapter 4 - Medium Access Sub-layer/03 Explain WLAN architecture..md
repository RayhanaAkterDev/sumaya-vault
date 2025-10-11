---
class: cse
title:
course:
  - Computer Network
chapter:
  - Chapter 4 - Medium Access Sub-layer
semester: 6th
date: 2025-09-06
status: pending 🛑
tags:
  - board_2019
  - board_2020
---


### **WLAN Architecture**

Wireless LANs (WLANs) let devices communicate **without cables** over a shared wireless network. The WLAN architecture is based on the **IEEE 802.11 standard**, so it is also called the **802.11 architecture**. It shows how **wireless devices, access points, and network systems** work together to provide reliable and secure communication.


1. **Basic Service Set (BSS)** – The BSS is the fundamental building block of a WLAN. It consists of a group of wireless stations (devices) that communicate with each other. There are two types of BSS:
    
    - **Independent BSS (IBSS)**: Also called an ad hoc network, where stations communicate directly without an access point.        
    - **Infrastructure BSS**: Stations communicate through an **Access Point (AP)**, which acts as a central hub.
        
2. **Access Point (AP)** – An AP is a device that connects wireless stations to the network and often to a wired LAN. It manages wireless traffic, provides authentication, and ensures smooth communication between wireless and wired devices.
    
3. **Extended Service Set (ESS)** – An ESS is formed when **multiple BSSs are connected via a distribution system (DS)**, typically a wired network. This allows mobility, as stations can move between BSSs while maintaining connectivity.
    
4. **Distribution System (DS)** – The DS is the backbone that interconnects multiple APs and BSSs. It handles **data forwarding, network management, and seamless roaming** across different BSSs in the ESS.
    
5. **Wireless Station (STA)** – A wireless device such as a laptop, smartphone, or IoT device that connects to the WLAN. Each STA communicates with other STAs either directly (in IBSS) or through an AP (in infrastructure mode).
    
6. **Service Areas** – Each AP defines a **coverage area called a Basic Service Area (BSA)**. Within this area, stations can communicate efficiently. Multiple overlapping BSAs allow seamless roaming for mobile devices.