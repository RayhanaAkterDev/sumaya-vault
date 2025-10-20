---
title: Github
class: note
date: 2025-10-05
tags: [code, git-github]
---

```dataview
table dateformat(file.ctime, "yyyy-MM-dd") as "Created", dateformat(file.mtime, "yyyy-MM-dd | hh:mm a") as "Modified"
from "@sandbox/@github"
where
  (
    length(split(file.folder, "/")) = length(split("@sandbox/@github", "/"))
    or (
      length(split(file.folder, "/")) = length(split("@sandbox/@github", "/")) + 1
      and contains(file.folder, file.name)
    )
  )
sort file.name asc
```