---
important links:
  - "[[@personal/Skin Care]]"
  - "[[@personal/Hair Care]]"
---

```dataview
table dateformat(file.day, "EEEE") as "Day", skin_care as "Skin Care", hair_care as "Hair Care"
from "02 Journal/Daily_Notes"
where contains(aliases, "skin_care") or contains(aliases, "hair_care")
sort file.day asc
```