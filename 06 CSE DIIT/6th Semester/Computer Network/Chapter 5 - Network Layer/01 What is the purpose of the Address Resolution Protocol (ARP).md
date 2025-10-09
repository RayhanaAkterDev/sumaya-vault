---
class: cse
title: 01 What is the purpose of the Address Resolution Protocol (ARP)?
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-08
status: pending 🛑
tags:
  - board_2019
  - board_2020
---

# Address Resolution Protocol (ARP)

### Introduction

Address Resolution Protocol (ARP) is a communication protocol used in IPv4 networks to map an IP address (logical address) to its corresponding MAC address (physical address). Since data transmission inside a local area network (LAN) happens using MAC addresses, ARP ensures that devices can locate each other and exchange data properly.

---

### Purpose of ARP

1. **Translate IP into MAC address**  
    The main purpose of ARP is to translate a known IP address into the correct MAC address of the destination device. This is necessary because IP addresses identify devices logically, but Ethernet frames require physical MAC addresses for actual delivery.
    
2. **Enable device communication in LAN**  
    ARP allows devices in the same local area network to communicate with each other smoothly. Without ARP, a computer would not know how to physically reach another device even if the IP address is known.
    
3. **Dynamic address resolution**  
    ARP provides an automatic method for discovering MAC addresses without requiring manual configuration. This makes networking flexible and reduces administrative overhead in managing devices.
    
4. **Maintain ARP cache for efficiency**  
    Once a device resolves an IP to a MAC address, it stores the result in an ARP cache. This avoids repeating the same broadcast request for future communications, making the process faster and more efficient.
    
5. **Use broadcast to discover unknown addresses**  
    If the MAC address of a destination is unknown, ARP sends a broadcast request to all devices in the LAN. The device with the matching IP address replies with its MAC, completing the mapping.
    
6. **Support IPv4-based networking**  
    ARP is a core protocol in IPv4 networks because Ethernet communication relies on MAC addresses. It ensures smooth data delivery at the link layer while still allowing higher-level protocols to work with IP addresses.
    
- **Assist in routing within subnets**  
    When data is sent within the same subnet, ARP ensures that the correct MAC address is identified so the data can be delivered locally. Without ARP, even packets within the same network could not be properly transmitted.
    
- **Provide transparency to higher layers**  
    ARP works in the background, making the process of IP-to-MAC mapping invisible to users and higher-level applications. This allows applications to use IP addresses without worrying about the underlying physical addressing.
    
- **Enable interoperability among devices**  
    ARP allows devices from different vendors and platforms to communicate as long as they support IPv4 and Ethernet. This ensures that mixed-device environments, such as PCs, printers, and servers, can exchange data seamlessly.
    

---

### Example of ARP in Action

Suppose Computer A with IP `192.168.1.2` wants to send data to Computer B with IP `192.168.1.5`. Computer A checks its ARP cache for the MAC address of Computer B. If it does not find it, A sends an ARP broadcast request. Computer B replies with its MAC address, which is then stored in A’s ARP cache. After that, Computer A can send data directly to Computer B using its MAC address.
