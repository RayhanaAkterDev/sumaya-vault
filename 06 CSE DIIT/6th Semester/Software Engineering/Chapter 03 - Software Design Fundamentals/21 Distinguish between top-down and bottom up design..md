---
class: cse
title: 21 Distinguish between top-down and bottom up design.
course:
  - Software Engineering
chapter:
  - "ch3: Software Design Fundamentals"
semester: 6th
date: 2025-09-05
status: pending 🛑
importance: ⭐⭐⭐⭐⭐
tags:
  - board_2018
  - board_2020
---

|Feature|Top-Down Design|Bottom-Up Design|
|---|---|---|
|**Definition**|Starts from the **high-level system overview** and breaks it down into smaller modules and components.|Starts from **low-level modules** and integrates them step by step to form higher-level systems.|
|**Approach**|**Decomposition approach:** System is divided into sub-modules progressively.|**Composition approach:** Small, functional modules are combined to build the system.|
|**Focus**|Focuses on **overall system design first**, then details.|Focuses on **detailed modules first**, then system integration.|
|**Module Testing**|High-level modules tested first; lower modules may require **stubs**.|Low-level modules tested first; higher modules integrated later using **drivers**.|
|**Ease of Development**|Requires clear understanding of the overall system upfront; may be harder if requirements are unclear.|Flexible, as low-level modules can be developed independently; easier for iterative development.|
|**Reusability**|Low-level modules may be less reusable initially since designed for specific top-level needs.|Low-level modules are highly reusable, as they are designed independently.|
|**Advantages**|Early validation of system’s main control and flow.|Promotes reusable modules; good for large systems with independent components.|
|**Disadvantages**|Late detection of lower-level module defects; stubs needed.|Full system may take time to be realized; top-level flow validated late.|