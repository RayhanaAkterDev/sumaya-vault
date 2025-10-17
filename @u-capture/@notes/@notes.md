---
title: Notes
class: note
---

# Table of Contents

```dataview
table dateformat(file.ctime, "yyyy-MM-dd") as "Created", file.mtime as "Modified"
from "@u-capture/@notes"
where length(split(file.folder, "/")) <= 2
sort file.name
```
