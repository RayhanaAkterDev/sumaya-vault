---
class: cse
title: 18 IPv6 next headers.
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - CN/Ch5
---
### IPv6 Next Headers

In IPv6, the concept of “Next Header” is used instead of the “Protocol” field in IPv4. The **Next Header field identifies the type of header immediately following the IPv6 header**. This mechanism allows IPv6 to support **extension headers** for optional network features, making the protocol more flexible and efficient.

**Example: **
If an IPv6 packet contains a **Hop-by-Hop Options header** followed by a **TCP segment**, the main IPv6 header’s Next Header field will point to the Hop-by-Hop header, and the Hop-by-Hop header’s Next Header field will point to TCP.

---

### Key Points About IPv6 Next Headers

- The **Next Header field** is an 8-bit field in the IPv6 header.    
- It **specifies the type of the following header**, which can be a **transport layer protocol** (like TCP, UDP) or an **extension header** (like Hop-by-Hop Options, Routing, Fragment).    
- Common values include **6 for TCP, 17 for UDP, 58 for ICMPv6**, and other values for various extension headers.    
- IPv6 allows **multiple extension headers** to be chained, with each header pointing to the next one using its own Next Header field.    
- Extension headers provide features such as **routing information, fragmentation, security (IPSec), and mobility**.    
- Routers only process specific headers relevant to them (e.g., Hop-by-Hop header), while other headers are passed along, improving **routing efficiency**.