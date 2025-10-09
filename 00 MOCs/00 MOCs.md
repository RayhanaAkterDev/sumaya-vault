---
Title: 🗺️ Master MOC
aliases: [Master MOC, Dashboard]
---

# 🗺️MOC Workspace

## 📂 MOC Index  

```dataview
table file.ctime as "Created"
from "00 MOCs"
where length(split(file.folder, "/")) <= 2
sort file.name asc
```

---

## 📁 Vault Overview

_This table shows your top-level folders with their creation dates._

```dataview
table file.folder as "Folder", dateformat(file.ctime, "yyyy-MM-dd") as "Created"
from ""
where length(split(file.folder, "/")) = 1
  and contains(file.path, file.folder + "/" + file.folder + ".md")
sort file.name asc
```
