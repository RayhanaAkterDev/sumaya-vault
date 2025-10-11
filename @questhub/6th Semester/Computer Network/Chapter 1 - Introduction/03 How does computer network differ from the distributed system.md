---
class: cse
title: 03 How does computer network differ from the distributed system
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-07-08
status: done ✅
importance: ⭐⭐⭐⭐⭐
tags:
  - board_2018
  - board_2021
topic: Topic 01 - Computer Network
---

## Computer Network & Distributed system

A **computer network** is a system where multiple computers or devices are interconnected through communication channels (such as cables, Wi-Fi, or optical fibers) to share data, hardware (like printers), and internet access. In a network, each computer operates **independently**, and communication is typically based on request-response without any central coordination for processing.

A **distributed system**, on the other hand, is a collection of independent computers that are connected via a network but work **collaboratively** to perform a single, unified task. These systems are designed to share computational power, storage, and processes in a coordinated manner. Although physically distributed, they appear as a **single coherent system** to the user, often providing higher fault tolerance, scalability, and performance.


## Differences between Computer Network & Distributed system

| **Aspect**             | **Computer Network**                                                                 | **Distributed System**                                                                 |
|------------------------|--------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|
| **Definition**         | A collection of interconnected computers that can communicate and share resources.  | A collection of independent computers that appears to users as a single coherent system. |
| **Goal**               | Enable communication and resource sharing between separate machines.                | Enable coordination and cooperation to achieve a common goal, making the collection behave like one. |
| **Autonomy**           | Each computer is autonomous and works independently, though connected.              | The system hides the distribution from the user, giving the illusion of a unified system. |
| **Transparency**       | No transparency; the user is aware of different computers and locations.            | High transparency; the system tries to hide the fact that multiple machines are involved. |
| **Examples**           | LAN, WAN, Internet                                                                  | Google’s distributed file system, cloud computing platforms                             |
| **Resource Management**| Managed individually on each machine.                                               | Resources are managed collectively by the distributed system software.                  |
| **Scalability**        | Limited to networking capabilities and bandwidth.                                   | Designed for high scalability, distributing workload across many nodes.                 |
| **Fault Tolerance**    | Failure of one computer usually affects only that computer.                         | Designed to hide individual component failures and ensure the system continues functioning as a whole. |
| **User View**          | Users see separate machines.                                                        | Users see a single, integrated system.                                                  |
| **Communication**      | Mainly about data exchange (emails, file sharing, messages).                        | Coordination of computation, data, and tasks across nodes to act like one powerful system. |

---
|**Computer Network**|**Distributed System**|
|---|---|
|A group of interconnected computers that communicate and share resources.|Independent computers working together, appearing as a single unified system to users.|
|Focused on enabling communication and sharing resources between machines.|Focused on coordinating tasks to act as a single coherent system.|
|Each computer operates independently.|The system conceals the distribution, giving the impression of one system.|
|Users are aware of different computers and locations.|The system hides the complexity, providing high transparency.|
|Examples include LAN, WAN, and the Internet.|Examples include Google’s distributed file system and cloud computing platforms.|
|Resources are managed separately on each machine.|Resources are managed collectively across the system.|
|Scalability is limited by network capacity and bandwidth.|Designed for high scalability, distributing workloads across multiple nodes.|
|Failure of one computer usually affects only that machine.|Failures are masked so the system continues functioning as a whole.|
|Users interact with separate machines.|Users perceive a single integrated system.|
|Mainly handles data exchange like emails and file sharing.|Coordinates computation, data, and tasks across nodes for unified operation.|