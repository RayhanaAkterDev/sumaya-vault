---
class: cse
title: 05 Draw and describe the fields of IPv6 header format.
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-08
status: pending 🛑
tags:
  - board_2018
---

# IPv6 Header Format

### Introduction

The **IPv6 header** is the fixed portion of an IPv6 packet that carries essential information for routing, delivery, and handling of the packet across networks. Unlike IPv4, the IPv6 header has a **fixed length of 40 bytes**, which simplifies processing by routers. It eliminates certain fields present in IPv4, such as checksum and fragmentation (which is handled by extension headers), making IPv6 more efficient for modern networking.

---

### IPv6 Header Diagram

```pgsql
  0                   8                  16                 31
+-------------------+-------------------+-------------------+
| Version | Traffic Class |       Flow Label                  |
+-------------------+-------------------+-------------------+
|         Payload Length         | Next Header | Hop Limit |
+----------------------------------------------------------+
|                   Source Address (128 bits)             |
+----------------------------------------------------------+
|               Destination Address (128 bits)           |
+----------------------------------------------------------+
```

---

### Description of IPv6 Header Fields

1. **Version (4 bits)**  
    Indicates the version of the Internet Protocol. For IPv6, this field is set to `6`. It allows devices and routers to interpret the packet correctly.
    
2. **Traffic Class (8 bits)**  
    Specifies the class of traffic or priority of the packet. Similar to the IPv4 Type of Service (ToS) field, it can be used for QoS (Quality of Service) purposes such as low-latency or high-throughput traffic.
    
3. **Flow Label (20 bits)**  
    Used to identify a sequence of packets requiring special handling, such as real-time streaming. Routers can use this field to provide consistent treatment of packets belonging to the same flow.
    
4. **Payload Length (16 bits)**  
    Indicates the length of the payload (data) following the header, in bytes. Unlike IPv4’s Total Length, it does **not include the header size**, because the header is fixed at 40 bytes.
    
5. **Next Header (8 bits)**  
    Identifies the type of header immediately following the IPv6 header. This could be a transport layer protocol like TCP (6) or UDP (17), or an extension header used for options such as routing, fragmentation, or security.
    
6. **Hop Limit (8 bits)**  
    Replaces the IPv4 TTL field. It specifies the maximum number of hops (routers) the packet can traverse. Each router decrements the hop limit by 1, and the packet is discarded if it reaches zero, preventing infinite circulation.
    
7. **Source Address (128 bits)**  
    Contains the IPv6 address of the sending device. It identifies the origin of the packet for routing and response purposes.
    
8. **Destination Address (128 bits)**  
    Contains the IPv6 address of the intended recipient. Routers use this to forward the packet toward its destination.
