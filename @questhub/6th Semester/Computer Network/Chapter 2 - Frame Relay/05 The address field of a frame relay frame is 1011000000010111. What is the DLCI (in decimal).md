---
class: cse
title: 05 The address field of a frame relay frame is 1011000000010111. What is the DLCI (in decimal)?
course:
  - Computer Network
chapter:
  - Chapter 2 - Frame Relay
semester: 6th
date: 2025-09-05
status: pending 🛑
importance: ⭐⭐⭐
tags:
  - board_2018
topic: "Topic 4: X.25 and Frame Relay"
---


> Note: _Checkout exam kit page no. 166_

The 16-bit Frame Relay address field is `1011000000010111`. To get the DLCI, we extract the relevant bits from both bytes of the address field. From the first byte, bits 1–6 (`101100`) correspond to 44 in decimal. From the second byte, bits 2–5 (`0010`) correspond to 2. Combining them: `(44 × 16) + 2 = 706`.

So, the DLCI in decimal is **706**.
