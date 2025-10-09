---
Title: Templates
---
`BUTTON[new_note]`
```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```

# Table of Contents

```dataview
table file.ctime as "Date"
from "10 Templates"
where length(split(file.folder, "/")) <= 2
sort file.name
```
