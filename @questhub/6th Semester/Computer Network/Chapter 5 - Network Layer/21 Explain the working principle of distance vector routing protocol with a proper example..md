---
class: cse
title: 21 Explain the working principle of distance vector routing protocol with a proper example.
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
# Distance Vector Routing Protocol

Distance Vector Routing Protocol is a type of **routing algorithm** used by routers to determine the best path to reach a network. It is based on the principle of **sharing routing information with immediate neighbors** and choosing paths based on distance (cost) metrics. Common examples of distance vector protocols include **RIP (Routing Information Protocol)** and **IGRP (Interior Gateway Routing Protocol)**.

---

**Working Principle:**  
The distance vector routing protocol works on the following principle:

1. Each router maintains a **routing table** that lists all known networks, the distance (usually in hops) to each network, and the next hop (neighboring router) to reach it.
    
2. Periodically, each router **shares its routing table with directly connected neighboring routers**.
    
3. When a router receives a routing table from a neighbor, it **updates its own table** by comparing the distance to each network via the neighbor with its current distance. If the new route offers a shorter distance, it replaces the old route.
    
4. This process continues until **all routers have consistent routing tables** and the shortest paths to all networks are known.
    
5. Distance vector protocols use **hop count as a metric**, and the maximum hop count is usually limited (e.g., 15 in RIP) to prevent routing loops.

---

**Example:**

Consider a network with three routers: **R1, R2, and R3**, connected as follows:

- R1 ↔ R2 ↔ R3

Initially:

- R1 knows only its directly connected networks.    
- R2 knows its networks and R1’s networks.    
- R3 knows its networks and R2’s networks.    

**Step 1:** R1 sends its routing table to R2. R2 compares R1’s table with its own and updates routes if a shorter path is found.

**Step 2:** R2 sends its updated routing table to R1 and R3. R1 and R3 update their tables based on new information.

**Step 3:** R3 sends its table to R2. R2 updates its table if any shorter paths exist.

After several iterations, all routers know the **shortest path to every network**. For instance, if a network N is directly connected to R3, R1 learns it via R2 → R3.