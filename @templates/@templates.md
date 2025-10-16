---
title: Templates
---

# Table of Contents

```dataview
list
from "@templates"
where length(split(file.folder, "/")) <= 2
sort file.name
```

---

```button
name Create template
type command
action Create new note
color blue
actions [{"type":"note text","action":""}]
```
^button-template