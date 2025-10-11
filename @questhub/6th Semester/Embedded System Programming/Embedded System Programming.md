---
Title: Embedded System Programming
course:
  - Embedded System Programming
semester: 6th
class: cse
date: 2025-08-04
status: pending ⏳
tags: ESP
---

`BUTTON[new_note]` 
```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```

### Chapter Notes

```dataview
table status as "Status"
from "06 CSE DIIT/6th Semester/Embedded System Programming"
where
  (
    length(split(file.folder, "/")) = length(split("06 CSE DIIT/6th Semester/Computer Network", "/"))
    or (
      length(split(file.folder, "/")) = length(split("06 CSE DIIT/6th Semester/Computer Network", "/")) + 1
      and contains(file.folder, file.name)
    )
  )
  
sort file.name asc
```