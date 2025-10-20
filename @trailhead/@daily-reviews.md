```dataview
table highlight, challenge, study_hour, code_hour , productivity_rating as productivity, tomorrow_focus
from "@journal/@daily-notes"
where contains(aliases, "daily-review")
sort file.day asc
```