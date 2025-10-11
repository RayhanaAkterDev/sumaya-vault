---
class: cse
title: 14 What is routing? Explain the working principle of any dynamic routing algorithm with a proper example.
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2022
---
### Routing

Routing is the process of **determining and selecting the optimal path for data packets to travel from a source device to a destination device across one or more networks**. It is a fundamental function in networking that enables devices in different networks to communicate with each other efficiently. Routing ensures that data is delivered correctly, avoiding unnecessary delays and congestion, by using devices like routers to examine the destination address of each packet and forward it through the most appropriate path.

Routing can be either **static**, where network paths are manually configured and remain fixed, or **dynamic**, where routes are automatically determined and updated based on current network conditions such as link failures, congestion, or topology changes.

**Example**  
A computer in one city sends data to a server in another city. Routers in the network decide the most efficient path for the data to reach the server.

---

To explain a dynamic routing algorithm, we can use the **Routing Information Protocol (RIP)**, a type of distance-vector algorithm.

RIP is one of the earliest and simplest dynamic routing algorithms based on the **distance-vector method**. It determines the best path for data transmission by using the **hop count** as its metric, where each router a packet passes through is considered one hop. The path with the fewest hops is chosen as the best route. Routers using RIP periodically exchange their routing tables with their neighbors, allowing the network to automatically update paths when changes occur.

**Working Principle of RIP:**

1. **Initialization:** Each router starts with a routing table containing only its directly connected networks, with a hop count of 0.
    
2. **Periodic Updates:** Every 30 seconds, each router broadcasts its complete routing table to all directly connected neighbors.
    
3. **Neighbor Updates:** Upon receiving updates, routers add 1 to each hop count and compare with their own entries. If a shorter path is found, the table is updated.
    
4. **Convergence:** Through continuous exchanges, routers eventually build a consistent and accurate view of the network topology.
    
5. **Path Selection:** When multiple paths to the same destination exist, the route with the lowest hop count is chosen.
    
6. **Loop Prevention:** RIP uses techniques like **split horizon** and **poison reverse** to avoid routing loops. A hop count of 16 is treated as infinity, marking the destination as unreachable.

**Example:**  
In a network of three routers (R1, R2, R3), R1 initially knows only its own connected network. After periodic updates, R1 learns from R2 that R3 is reachable in 2 hops. R1 updates its table, choosing the shortest path automatically.