---
class: cse
title: 20 Distinguish between classless and class full IP addressing.
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
# Distinction Between Classful and Classless IP Addressing

| Feature                | Classful IP Addressing                                                                             | Classless IP Addressing (CIDR)                                                                    |
| ---------------------- | -------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| **Network Division**   | Divides IP space into fixed classes (A, B, C, D, E) with predetermined network and host portions.  | Uses variable-length network prefixes, allowing flexible division of network and host portions.   |
| **Address Efficiency** | Often wastes IP addresses because networks may not match class sizes exactly.                      | Efficient use of IP addresses; allocates only the number of addresses required.                   |
| **Routing**            | Routing tables can become large as each class is handled separately.                               | Supports route aggregation (summarization), reducing routing table size.                          |
| **Flexibility**        | Low flexibility due to fixed classes.                                                              | High flexibility with subnetting and supernetting.                                                |
| **Subnetting**         | Subnetting is limited; network and host boundaries are fixed by class.                             | Subnetting is fully flexible; network administrators can create subnets of any size.              |
| **Scalability**        | Not suitable for large or growing networks due to wasted addresses and rigid structure.            | Highly scalable; can accommodate networks of varying sizes efficiently.                           |
| **Compatibility**      | Only supports IPv4; obsolete for modern internet.                                                  | Supports IPv4 and can be adapted to IPv6; widely used in modern networking.                       |
| **Security**           | Class boundaries can sometimes make access control less flexible.                                  | Allows precise allocation and separation of subnets, improving network segmentation and security. |
| **Example**            | A company needing 200 addresses would require a Class C network (254 hosts), wasting 54 addresses. | The same company can use a /24 or /25 subnet, allocating exactly 200 addresses efficiently.       |
| **Usage**              | Mostly used in early IP networks.                                                                  | Standard in modern networks and internet routing.                                                 |