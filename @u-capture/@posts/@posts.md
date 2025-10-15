---
Title: NoteLab
---
`BUTTON[new_note]`
```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```

# Table of Contents

```dataview
table dateformat(file.ctime, "yyyy-MM-dd") as "Created"
from "08 LinkedIn"
where length(split(file.folder, "/")) <= 2
sort file.name
```
