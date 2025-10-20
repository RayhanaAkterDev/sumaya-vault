---
title: Tailwind Cheat Sheets
class: note
date: 2025-10-07
tags:
  - tailwind
  - cheatsheet
---

## Tailwind Cheat Sheets

```dataview
list
from "@sandbox/@tailwind/@cheatsheet"
where
  (
    length(split(file.folder, "/")) = length(split("@sandbox/@tailwind/@cheatsheet", "/"))
    or (
      length(split(file.folder, "/")) = length(split("@sandbox/@tailwind/@cheatsheet", "/")) + 1
      and contains(file.folder, file.name)
    )
  )
sort file.name asc
```