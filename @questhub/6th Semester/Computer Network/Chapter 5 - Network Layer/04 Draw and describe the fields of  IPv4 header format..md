---
class: cse
title: 04 Draw and describe the fields of  IPv4 header format.
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-08
status: pending 🛑
tags:
  - board_2021
  - board_2022
---

# IPv4 Header Format

An **IPv4 header** is the portion of an IPv4 packet that contains control information needed for routing, delivery, and handling of the packet. It precedes the data (payload) in the packet and typically has a minimum size of **20 bytes** (without options) and a maximum size of **60 bytes** (with options).

**IPv4 Header Diagram**

```pgsql
  0                   8                  16                 31
+-------------------+-------------------+-------------------+
| Version | IHL     | Type of Service (ToS)                     |
+-------------------+-------------------+-------------------+
| Total Length                                         |
+------------------------------------------------------+
| Identification                                      |
+-------------------+-------------------+--------------+
| Flags             | Fragment Offset                   |
+-------------------+-------------------+--------------+
| Time to Live (TTL) | Protocol           | Header Checksum|
+------------------------------------------------------+
| Source IP Address                                     |
+------------------------------------------------------+
| Destination IP Address                                |
+------------------------------------------------------+
| Options (if any) + Padding                            |
+------------------------------------------------------+
```

### Description of IPv4 Header Fields

1. **Version (4 bits)**  
    This field specifies the version of the Internet Protocol used. For IPv4 packets, the value is set to `4`. Routers and receiving devices use this field to identify how to interpret the rest of the packet, ensuring proper processing of IPv4 data.
    
2. **IHL (Internet Header Length, 4 bits)**  
    The IHL field indicates the length of the IP header in 32-bit words. The minimum length is 5 words (20 bytes), which corresponds to a header without options. This field allows the receiver to determine where the payload data begins, which is important when options are included.
    
3. **Type of Service (ToS, 8 bits)**  
    Also known as the **Differentiated Services field**, this field specifies the priority and quality of service for the packet. It can define parameters such as delay, throughput, reliability, and cost, helping routers handle the packet according to network policies and optimize delivery.
    
4. **Total Length (16 bits)**  
    This field specifies the total size of the IP packet, including both header and data, in bytes. The maximum size is 65,535 bytes. This information is critical for the receiver to determine where the packet ends and for routers to handle fragmentation when needed.
    
5. **Identification (16 bits)**  
    The identification field uniquely labels each packet sent by a source. This is especially important when a packet is fragmented during transmission; the identification number allows the receiver to reassemble fragments in the correct order to reconstruct the original packet.
    
6. **Flags (3 bits)**  
	The **Flags** field is 3 bits long and is used to control or identify fragmentation of IP packets. Each bit has a specific role:
	- **Bit 0:** Reserved – always set to `0`.
    - **Bit 1:** DF (Don't Fragment) – if set, prevents the packet from being fragmented.
    - **Bit 2:** MF (More Fragments) – if set, indicates that more fragments of this packet follow; if cleared, this is the last fragment.
    The Flags field works together with the **Fragment Offset** field to ensure correct fragmentation and reassembly of packets when the packet size exceeds the network’s Maximum Transmission Unit (MTU).
    
7. **Fragment Offset (13 bits)**  
    This field specifies the position of a particular fragment relative to the start of the original packet. It allows the receiver to correctly reassemble fragmented packets into their original sequence, ensuring that large messages can be transmitted even if the network limits individual packet size.
    
8. **Time to Live (TTL, 8 bits)**  
    The TTL field sets the maximum lifetime of a packet in the network. Each router that forwards the packet decreases the TTL by 1. If TTL reaches 0, the packet is discarded to prevent it from circulating indefinitely due to routing loops.
    
9. **Protocol (8 bits)**  
    This field indicates the type of transport layer protocol carried in the payload of the IP packet. For example, `6` represents TCP, `17` represents UDP, and `1` represents ICMP. The protocol field allows the receiver to correctly interpret the encapsulated data.
    
10. **Header Checksum (16 bits)**  
    This field contains a checksum calculated over the IP header to detect errors during transmission. Routers and receivers recalculate the checksum and discard packets if errors are detected, ensuring the integrity of control information in the header.
    
11. **Source IP Address (32 bits)**  
    This field contains the IP address of the sender. It identifies the origin of the packet, allowing responses to be routed back to the correct source device. It is essential for end-to-end communication across networks.
    
12. **Destination IP Address (32 bits)**  
    This field specifies the IP address of the intended recipient. Routers use this address to forward the packet toward its destination, making it the key element in packet delivery.
    
13. **Options (Variable)**
	The **Options** field is optional and can vary in length. It provides additional control features such as:
	- Security parameters
	- Record route (keeps track of the path the packet takes)
    - Timestamp (records the time the packet passes through a router)
    This field is not always used; it is mainly for special purposes or network management.
    
14. **Padding (Variable)**
	The **Padding** field ensures that the IPv4 header is always a multiple of 32 bits. If the **Options** field does not align to 32-bit boundaries, padding bytes (set to `0`) are added to fill the space. This ensures proper alignment for processing by routers and receiving devices.