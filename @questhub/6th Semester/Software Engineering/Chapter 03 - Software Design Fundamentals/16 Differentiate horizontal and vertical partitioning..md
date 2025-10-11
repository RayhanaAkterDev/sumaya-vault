---
class: cse
title: 16 Differentiate horizontal and vertical partitioning.
course:
  - Software Engineering
chapter:
  - "ch3: Software Design Fundamentals"
semester: 6th
date: 2025-09-05
status: pending 🛑
importance: ⭐⭐
tags:
  - board_2017
  - board_2019
---

|Aspect|Horizontal Partitioning|Vertical Partitioning|
|---|---|---|
|**Definition**|Divides a table **row-wise**, creating partitions with subsets of rows.|Divides a table **column-wise**, creating partitions with subsets of columns.|
|**Purpose**|Improves query performance and load balancing by storing different rows on different servers.|Optimizes storage and reduces I/O by retrieving only necessary columns.|
|**Partition Basis**|Based on row values, ranges, or specific conditions.|Based on column usage, grouping frequently accessed and less-used columns.|
|**Usage**|Useful when queries frequently access a subset of rows.|Useful when queries frequently access only specific columns.|
|**Focus**|Splits data **across rows**.|Splits data **across columns**.|
|**Data Distribution**|Each partition contains all columns but only some rows.|Each partition contains all rows but only some columns.|
|**Performance Impact**|Reduces query load by limiting the number of rows scanned.|Reduces query load by limiting the number of columns scanned.|
|**Storage Location**|Partitions can be stored on different servers or disks.|Partitions are usually stored on the same server but can also be distributed.|
|**Complexity**|Generally simpler to implement in distributed systems.|Requires careful planning of column grouping; can be more complex.|
|**Scalability**|Better scalability for large datasets accessed row-wise.|Better optimization for queries targeting specific attributes.|
