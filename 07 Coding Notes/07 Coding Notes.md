---
title: Coding Notes
class: note
tags:
  - code
---

`BUTTON[new_note]` 

```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```

---

### Folder Notes

```dataview
list
from "07 Coding Notes"
where contains(file.folder, file.name)
  and length(split(file.folder, "/")) = length(split("07 Coding Notes", "/")) + 1
sort file.ctime asc
```