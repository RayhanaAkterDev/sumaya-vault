---
class: cse
title: 30 What is cellular network? Explain handover process in the cellular networks.
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-08-04
status: pending 🛑
tags:
  - CN/Ch1/board_2021
---

## Cellular Network

A cellular network is a type of wireless communication system that divides a large geographical area into smaller regions called _cells_. Each cell is served by a base station equipped with antennas and radio transmitters, which connect mobile devices to the network. These base stations are linked to a central Mobile Switching Center (MSC), which manages call routing, mobility, and resource allocation. The main advantage of this structure is **frequency reuse**, where the same radio frequencies can be used in non-adjacent cells, increasing capacity and coverage. Cellular networks provide seamless voice, data, and internet services while ensuring mobility, allowing users to stay connected even when moving from one place to another.

---

## Handover Process in Cellular Networks

1. **Measurement**  
    The handover process starts with the mobile device continuously monitoring the signal strength and quality of both the current cell and neighboring cells. This information is regularly sent to the network so it can assess connection quality and detect when the current signal is weakening.
    
2. **Decision**  
    Based on the measurement reports, the network decides whether a handover is necessary. The decision considers factors like a weaker signal from the current cell, a stronger signal from a neighboring cell, or balancing network traffic to maintain good service quality. This ensures that the user’s communication remains uninterrupted and of high quality.
    
3. **Execution**  
    Once the decision is made, the network prepares the new connection and instructs the mobile device to switch to the target cell. After a successful switch, the old connection is released. This smooth transition allows calls and data sessions to continue without noticeable interruption.