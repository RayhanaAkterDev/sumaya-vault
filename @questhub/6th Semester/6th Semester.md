---
title: 6th Semester
class: cse
semester: 6th
status: working 🚀
date: 2025-07-27
---

### Courses


```dataview
table status as "Status"
from "@questhub/6th Semester"
where contains(file.folder, file.name)
  and length(split(file.folder, "/")) = length(split("@questhub/6th Semester", "/")) + 1
sort file.name asc
```
