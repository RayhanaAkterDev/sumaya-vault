---
class: cse
title: Embedded System Programming Final Suggestion
course: Embedded System Programming
chapter:
semester: 6th
date: 2025-09-20
status: working 🚀
tags:
  - ESP
---
```dataview
table chapter as "Chapter", topic as "Topic", importance as "Rating", join(map(tags, (t) => "• [#" + t + "](#" + t + ")"), "<br>") as "Tags"
from "06 CSE DIIT/6th Semester/Embedded System Programming"
where chapter and topic
sort !chapter, chapter, topic, importance desc
```
