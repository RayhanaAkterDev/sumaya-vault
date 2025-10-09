---
class: cse
title: 09 Explain the shortest path routing.
course:
  - Computer Network
chapter:
  - Chapter 5 - Network Layer
semester: 6th
date: 2025-09-11
status: pending 🛑
tags:
  - board_2017
---
### Shortest Path Routing

Shortest Path Routing is a routing technique in which the route selected between the source and destination is the one with the **minimum cost**. The cost may be measured in terms of distance, number of hops, transmission delay, or any other metric that reflects the efficiency of a path. The main objective of shortest path routing is to deliver data packets using the most optimal and efficient path available in the network.

---

### Working Principle:

- Each router in the network maintains information about its neighbors and the cost of links connecting to them.
    
- A **routing algorithm** (commonly Dijkstra’s algorithm) is used to compute the shortest path from the router to all other nodes in the network.
    
- The cost of a path is calculated by summing up the weights (such as hop count, distance, or delay) of the links along that path.
    
- Once the shortest paths are calculated, the results are stored in the **routing table**, which is then used to forward packets toward their destination.

![[Pasted image 20250911163626.png]]