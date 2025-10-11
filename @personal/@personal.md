---
Title: NoteLab
---
`BUTTON[new_note]`
```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```

# Table of Contents

```dataview
table dateformat(file.ctime, "yyyy-MM-dd") AS Created
from "@personal"
where length(split(file.folder, "/")) <= 2
sort file.name
```
