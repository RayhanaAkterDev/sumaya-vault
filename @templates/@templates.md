---
Title: Templates
---

# Table of Contents

```dataview
list
from "@templates"
where length(split(file.folder, "/")) <= 2
sort file.name
```

---

`BUTTON[new_note]`

```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```