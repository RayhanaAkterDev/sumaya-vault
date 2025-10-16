---
Title: Computer Network
course:
  - Computer Network
semester: 6th
class: cse
date: 2025-08-04
status: working 🚀
tags: CN
---

`BUTTON[new_note]` 
```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```

### Chapter Notes

```dataview
table status as "Status", tags
from "@questhub/6th Semester/Computer Network"
where
  (
    length(split(file.folder, "/")) = length(split("@questhub/6th Semester/Computer Network", "/"))
    or (
      length(split(file.folder, "/")) = length(split("@questhub/6th Semester/Computer Network", "/")) + 1
      and contains(file.folder, file.name)
    )
  )
sort file.name asc
```
