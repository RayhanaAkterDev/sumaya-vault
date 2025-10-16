---
class: cse
title: Peripheral & Interfacing
course:
  - Peripheral & Interfacing
chapter:
  - chapter 1 - Interfacing Techniques
semester: 5th
tags:
  - cse
  - study
  - 5th_sem
---

## Peripheral & Interfacing Chapters

```dataview
list
FROM "@questhub/5th Semester/01 Peripheral & Interfacing"
where
  (
    length(split(file.folder, "/")) = length(split("@questhub/5th Semester/01 Peripheral & Interfacing", "/"))
    or (
      length(split(file.folder, "/")) = length(split("@questhub/5th Semester/01 Peripheral & Interfacing", "/")) + 1
      and contains(file.folder, file.name)
    ) and file.name != "01 Peripheral & Interfacing"
  )
sort file.name asc
```
