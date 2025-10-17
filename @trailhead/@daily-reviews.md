```dataview
table highlight, challenge, lesson, proud_task, tomorrow_focus, productivity_rating as productivity
from "@journal/@daily-notes"
where contains(aliases, "daily-review")
sort file.day asc
```