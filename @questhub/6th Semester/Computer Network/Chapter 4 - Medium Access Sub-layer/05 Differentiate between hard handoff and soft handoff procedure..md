---
class: cse
title: 05 Differentiate between hard handoff and soft handoff procedure.
course:
  - Computer Network
chapter:
  - Chapter 4 - Medium Access Sub-layer
semester: 6th
date: 2025-09-06
status: pending 🛑
tags:
  - board_2020
---

## Difference Between Hard Handoff and Soft Handoff

|Feature|Hard Handoff|Soft Handoff|
|---|---|---|
|**Definition**|The mobile device **disconnects from the current base station before connecting to the next one**.|The mobile device **connects to the new base station while still maintaining connection with the current one**.|
|**Connection Type**|**Break-before-make**: connection is broken first, then made with the new station.|**Make-before-break**: connection with the new station is established before breaking the old one.|
|**Interruption**|Can cause a **brief interruption** in communication.|Usually **seamless**, with no interruption.|
|**Usage**|Common in **GSM (2G) cellular networks**.|Common in **CDMA (3G) cellular networks**.|
|**Complexity**|Simple to implement.|More complex due to simultaneous multiple connections.|
|**Reliability**|Less reliable during handoff; higher **chance of call drop**.|More reliable; **low chance of call drop** due to overlapping connections.|
|**Signal Handling**|Only one signal path at a time; signal quality can temporarily drop.|Multiple signal paths are used; **better signal quality and stability**.|
|**Latency**|Slightly higher latency due to reconnection process.|Lower latency; smooth transition because the old connection is maintained.|
|**Resource Usage**|Requires fewer network resources as only one connection exists at a time.|Requires more network resources as multiple connections are maintained simultaneously.|
|**Handoff Speed**|Faster to switch once connection is broken, but riskier.|Slightly slower due to managing multiple connections, but safer.|