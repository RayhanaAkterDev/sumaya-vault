---
title: Tailwind Cheat Sheets
class: note
date: 2025-10-07
tags:
  - tailwind
  - cheatsheet
---

`BUTTON[new_note]` 

```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```

---

## Tailwind CheatSheets

```dataview
list
from "07 Coding Notes/Tailwind 4.0/Cheat Sheets"
where
  (
    length(split(file.folder, "/")) = length(split("07 Coding Notes/Tailwind 4.0/Cheat Sheets", "/"))
    or (
      length(split(file.folder, "/")) = length(split("07 Coding Notes/Tailwind 4.0/Cheat Sheets", "/")) + 1
      and contains(file.folder, file.name)
    )
  )
sort file.name asc
```