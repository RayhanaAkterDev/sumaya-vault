---
class: cse
title: 01 Explain the CSMA/CD technique (with flow-chart) to access a medium.
course:
  - Computer Network
chapter:
  - Chapter 4 - Medium Access Sub-layer
semester: 6th
date: 2025-09-06
status: pending 🛑
tags:
  - board_2018
  - board_2021
---

## CSMA/CD Technique

Carrier Sense Multiple Access with Collision Detection (CSMA/CD) is a **media access control protocol** used in traditional Ethernet networks (IEEE 802.3) to control access to a shared communication medium. Its main purpose is to **avoid data collisions** when multiple stations attempt to send data at the same time.

![[CD-Flow-Chart-new.png]]

## Working Process of CSMA/CD

1. **Carrier Sensing** – Each station first listens to the medium to check if it is idle. If the medium is busy, the station waits until it becomes free, ensuring that it does not interfere with any ongoing transmission. This step helps in reducing the chances of collisions on the network.
    
2. **Data Transmission** – Once the medium is idle, the station begins transmitting its data frame. While transmitting, it continues to monitor the medium to detect any collision that may occur due to simultaneous transmissions by other stations.
    
3. **Collision Detection** – If two or more stations transmit at the same time, their signals overlap, causing a collision. The station detects this by observing that the signal on the medium differs from what it is sending, indicating that multiple transmissions are interfering.
    
4. **Jam Signal** – Upon detecting a collision, the stations immediately stop transmitting and send a short jam signal. This signal spreads across the network to ensure that all stations are aware of the collision and can take appropriate action.
    
5. **Backoff Process** – After sending the jam signal, each station waits for a random backoff time before attempting retransmission. The backoff time is calculated using the **Binary Exponential Backoff algorithm**, which helps in minimizing repeated collisions by introducing different waiting periods for each station.
    
6. **Retransmission** – Once the backoff period expires, the station senses the medium again. If it is idle, it retransmits the frame. This process repeats as necessary until the data is successfully transmitted without collision, ensuring reliable communication over the shared medium.