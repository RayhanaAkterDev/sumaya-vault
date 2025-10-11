---
Title: Vault Index
---

# 📁 Vault Index

_This table shows your top-level folders with their creation dates._

```dataview
list
from ""
where length(split(file.folder, "/")) = 1
  and contains(file.path, file.folder + "/" + file.folder + ".md")
sort file.name asc
```
