---
class: cse
title: 5th Semester
semester: 5th
tags:
  - cse
  - study
  - 5th_sem
---

## 5th Semester Course List

```dataview
list
from "@questhub/5th Semester"
where contains(file.folder, file.name)
  and length(split(file.folder, "/")) = length(split("@questhub/5th Semester", "/")) + 1
sort file.name asc
```