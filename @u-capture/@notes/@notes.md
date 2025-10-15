---
title: 01 NoteLab
class: note
---
`BUTTON[quick_note]` 

```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```

# Table of Contents

```dataview
table dateformat(file.ctime, "yyyy-MM-dd") as "Created", file.mtime as "Modified"
from "01 NoteLab"
where length(split(file.folder, "/")) <= 2
sort file.name
```
