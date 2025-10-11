---
class: cse
title: 02 What is IP addresses?
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

# IP Address

An **Internet Protocol (IP) address** is a structured numerical label assigned to each device connected to a computer network that uses the Internet Protocol for communication. It serves two essential roles: first, as a **unique identifier** for the device (like a roll number for a student), and second, as a **locator** that specifies where the device is situated within the network. An IP address is embedded into every data packet, where the **source IP** indicates the sender’s address and the **destination IP** indicates the receiver’s address. This allows routers and switches to forward the packet correctly across local networks and the Internet. In short, the IP address acts like the digital address of a device, ensuring accurate identification and delivery of data between millions of interconnected systems worldwide.

**Example**

- **IPv4 example:** `192.168.1.10` – typically used in home and office LANs.    
- **IPv6 example:** `2001:0db8:85a3:0000:0000:8a2e:0370:7334` – designed for modern networks with far more devices.  

---

### Key Characteristics of IP Addresses

1. **Uniqueness** – Each device in a network must have a distinct IP address to avoid confusion and ensure data is delivered to the right destination.
    
2. **Hierarchical structure** – IP addresses are divided into a network portion and a host portion, which allows easy identification of both the network and the specific device.
    
3. **Two versions** – IPv4 uses 32-bit addresses written in dotted-decimal format, while IPv6 uses 128-bit addresses written in hexadecimal format separated by colons.
    
4. **Types of usage** – IP addresses can be public (used globally on the Internet) or private (used within local networks such as homes, offices, or organizations).
    
5. **Formats** – IPv4 looks like `192.168.1.1` (four octets), whereas IPv6 looks like `fe80::1ff:fe23:4567:890a` (eight groups of hexadecimal).
    
6. **Assignment method** – They can be static (manually configured and fixed) or dynamic (automatically assigned by DHCP servers for temporary use).
    
7. **Fundamental for routing** – Routers depend on IP addresses to determine the correct path for data packets across networks, making them the backbone of Internet communication.
