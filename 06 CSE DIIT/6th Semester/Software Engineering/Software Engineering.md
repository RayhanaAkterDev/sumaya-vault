---
Title: Software Engineering
course: Software Engineering
semester: 6th
class: cse
date: 2025-08-04
status: pending ⏳
tags: SE
---

`BUTTON[new_note]` 
```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```

### Chapter Notes

```dataview
table status as "Status"
from "06 CSE DIIT/6th Semester/Software Engineering"
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
