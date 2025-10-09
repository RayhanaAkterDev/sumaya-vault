---
class: cse
title: For NU Final Exam Preparation of Computer Network
course:
  - Computer Network
chapter:
semester: 6th
date: 2025-09-17
status: working 🚀
tags:
  - CN
---
```dataview
table chapter as "Chapter", topic as "Topic", importance as "Rating", join(map(tags, (t) => "• [#" + t + "](#" + t + ")"), "<br>") as "Tags"
from "06 CSE DIIT/6th Semester/Computer Network"
where chapter and topic
sort !chapter, chapter, topic, file.name asc
```
