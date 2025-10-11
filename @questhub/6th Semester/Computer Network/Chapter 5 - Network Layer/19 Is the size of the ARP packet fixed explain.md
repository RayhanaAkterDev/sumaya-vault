---
class: cse
title: 19 Is the size of the ARP packet fixed explain
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-07
status: pending 🛑
tags:
  - CN/Ch5
---
# Address Resolution Protocol (ARP) Packet Size

ARP (Address Resolution Protocol) is used to map a device’s **IP address** to its **MAC address** on a local network. Each ARP packet contains fields that carry information about the sender and target addresses, operation type, and hardware/protocol types.

---

**Is the ARP Packet Size Fixed?**  

No, the size of an ARP packet is **not entirely fixed**; it can vary slightly depending on the types and lengths of addresses used. However, in most common implementations on Ethernet networks using IPv4:

**Standard Ethernet/IPv4 ARP Packet Size:**
    - Hardware type: 2 bytes        
    - Protocol type: 2 bytes        
    - Hardware address length: 1 byte        
    - Protocol address length: 1 byte        
    - Operation code: 2 bytes        
    - Sender MAC address: 6 bytes        
    - Sender IP address: 4 bytes        
    - Target MAC address: 6 bytes        
    - Target IP address: 4 bytes
    
   The total is **28 bytes** for the ARP payload. When encapsulated in an Ethernet frame, the total frame size becomes **42 bytes minimum** (including Ethernet header).

----

 **Why Size Can Vary:**

If ARP is used on a network with **different hardware types or protocol addresses**, the **hardware and protocol address lengths** can change. For example, ARP can theoretically work with longer hardware addresses than Ethernet’s 6 bytes, or IPv6 (via NDP) uses 16-byte addresses, changing the packet structure.