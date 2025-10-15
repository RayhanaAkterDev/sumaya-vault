# Table of Contents

```dataview
table dateformat(file.ctime, "yyyy-MM-dd") as "Created", file.mtime as "Modified"
from "Software Lab Project/Project Progress"
where length(split(file.folder, "/")) <= 2
sort file.name
```

---

`BUTTON[new_note]` 
```meta-bind-embed
[[MetaBindEmbeds Spaces Buttons]]
```