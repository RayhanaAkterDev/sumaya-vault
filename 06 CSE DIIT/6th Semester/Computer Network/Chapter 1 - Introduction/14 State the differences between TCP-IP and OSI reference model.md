---
class: cse
title: 14 State the differences between TCP/IP and OSI reference model
course:
  - Computer Network
chapter:
  - chapter 1 - Introduction
semester: 6th
date: 2025-07-08
status: done ✅
tags:
  - CN/Ch1/board_2018
---

|**Aspect**|**TCP/IP Model**|**OSI Model**|
|---|---|---|
|**Origin and Purpose**|Developed by the U.S. Department of Defense for practical use in networking and the internet. It is designed based on protocols that are already in use.|Developed by ISO as a theoretical framework to guide and standardize networking protocols universally. Mainly used for learning and understanding network communication.|
|**Number of Layers**|Has 4 layers: Application, Transport, Internet, and Network Access (combines data link and physical).|Has 7 layers: Application, Presentation, Session, Transport, Network, Data Link, and Physical, with each layer performing a specific function.|
|**Layer Functions**|Combines several functions such as session and presentation into the Application layer for simplicity and practicality.|Clearly separates functions like presentation (data formatting) and session (managing connections) into separate layers for modularity and clarity.|
|**Protocol Dependency**|Protocol-dependent model specifying protocols like TCP, IP, UDP, HTTP, FTP, etc.|Protocol-independent reference model that does not specify any protocols but acts as a guideline.|
|**Usage in Practice**|Widely used as the foundation of the internet and real-world networking systems.|Primarily used as a teaching tool and reference model to help understand and design network systems.|
|**Communication Style**|Supports both connection-oriented communication (TCP) and connectionless communication (UDP).|Communication style depends on the protocols implemented within the layers, as OSI is conceptual.|
|**Flexibility and Complexity**|Simpler with fewer layers, making it easier to implement but less flexible in terms of strict layering.|More detailed and modular, allowing flexibility but can be more complex to implem|

