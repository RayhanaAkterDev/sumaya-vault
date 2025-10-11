---
title: Tailwind 4.0
class: note
date: 2025-10-05
tags:
  - code
  - tailwind
---

`BUTTON[new_note]` 

```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```

---

## Tailwind 4.0 All Notes

```dataview
table dateformat(file.ctime, "yyyy-MM-dd") as "Created", dateformat(file.mtime, "yyyy-MM-dd | hh:mm a") as "Modified"
from "07 Coding Notes/Tailwind 4.0"
where
  (
    length(split(file.folder, "/")) = length(split("07 Coding Notes/Tailwind 4.0", "/"))
    or (
      length(split(file.folder, "/")) = length(split("07 Coding Notes/Tailwind 4.0", "/")) + 1
      and contains(file.folder, file.name)
    )
  )
sort file.name asc
```