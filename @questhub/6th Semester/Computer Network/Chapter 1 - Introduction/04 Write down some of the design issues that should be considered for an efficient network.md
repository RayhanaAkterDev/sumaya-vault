---
class: cse
title: 04 Write down some of the design issues that should be considered for an efficient network
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-07-08
status: done ✅
importance: ⭐⭐⭐
tags:
  - board_2017
topic: Topic 01 - Computer Network
---

## Here are some key **design issues** that should be considered to build an **efficient computer network**

> 1. **Performance**: The network should handle data quickly and reliably, with low delay and minimal data loss, ensuring smooth communication for all users.

> 2. **Scalability**: It must allow easy expansion to support more devices or users without major changes or a drop in performance.

> 3. **Security**: Protecting the network from unauthorized access, attacks, and data theft through encryption, firewalls, and access controls is essential.

> 4. **Reliability**: The network should continue working properly even if some devices fail, using backup paths and fault-tolerant designs to avoid downtime.

> 5. **Cost-effectiveness**: A good network balances performance and reliability with reasonable costs for equipment, installation, and maintenance.

> 6. **Manageability**: The network should be easy to configure, monitor, and troubleshoot using appropriate tools and software.

> 7. **Bandwidth Utilization**: Sufficient bandwidth is needed to support data traffic without congestion, ensuring users get consistent speeds.

> 8. **Quality of Service (QoS)**: The network should prioritize critical or time-sensitive data (like voice or video) to maintain good quality even under heavy use.

> 9. **Topology**: Choosing the right physical or logical layout (such as star, mesh, or bus) helps improve performance, fault tolerance, and maintenance.

> 10. **Interoperability** (আন্তঃকার্যক্ষমতা): The network devices and protocols should follow standards to ensure compatibility and smooth communication between different equipment.

---

## ✅ Design Issues of the Network Layer

The **network layer** is responsible for routing and delivering data packets from source to destination across multiple networks. The main design issues of this layer include:

> 1. **Routing**: The most critical function. It deals with choosing the best path for data packets to travel from the sender to the receiver across many possible routes. Algorithms must consider factors like distance, congestion, and speed while updating routes dynamically.

> 2. **Addressing**: Every device in a network must have a unique IP address. The network layer assigns addresses that help identify the source and destination of data packets. Both logical (IP) and physical (MAC) addresses are important for communication.

> 3. **Packet Forwarding**: After determining the route, the network layer forwards the data to the next device (router or destination). Routers use forwarding tables to decide where to send each packet based on its destination IP address.

> 4. **Internetworking**: This involves connecting different types of networks (LAN, MAN, WAN) and ensuring that data can flow seamlessly between them. The network layer must handle differences in addressing, protocols, and frame formats.

> 5. **Congestion Control**: When too much data is sent over the network, congestion can occur, causing delays and packet loss. The network layer must detect and reduce congestion by slowing traffic or rerouting packets.

> 6. **Fragmentation and Reassembly**: If a packet is too large for the next network, it must be broken into smaller pieces (fragments). The network layer ensures that these fragments are reassembled at the destination in the correct order.

> 7. **Error Handling and Reporting**: The network layer detects delivery problems, such as unreachable destinations or timeouts, and reports them using protocols like ICMP (Internet Control Message Protocol).

> 8. **Sequencing**: When a packet is divided into fragments, the network layer numbers each fragment so that they can be reassembled correctly at the receiving end, maintaining the original data sequence.
