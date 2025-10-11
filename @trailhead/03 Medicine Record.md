```dataview
table Thyrox-50, Xinc-B, E-Cap
from "02 Journal/Daily_Notes"
where contains(aliases, "medicine_record")
sort file.day asc
```