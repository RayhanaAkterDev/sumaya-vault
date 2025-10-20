---
title: Sandbox
class: note
aliases:
  - Coding Note
tags:
  - code
---
 `button-note` 

---
```dataview
list
from "@sandbox"
where contains(file.folder, file.name)
  and length(split(file.folder, "/")) = length(split("@sandbox", "/")) + 1
sort file.ctime asc
```