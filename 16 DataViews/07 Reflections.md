```dataview
table rating as "Rating", join(map(split(reflection, ","), (x) => "• " + x), "<br>") as Reflection
from "02 Journal/Daily_Notes"
where contains(aliases, "reflection")
sort file.day asc
```