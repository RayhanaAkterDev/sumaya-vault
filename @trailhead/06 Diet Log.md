```dataview
table 
  join(map(split(breakfast, ","), (x) => "• " + x), "<br>") as breakfast,
  join(map(split(snacks, ","), (x) => "• " + x), "<br>") as Snacks,
  join(map(split(lunch, ","), (x) => "• " + x), "<br>") as Lunch,
  join(map(split(dinner, ","), (x) => "• " + x), "<br>") as Dinner,
  dinner_by_7,
  sugar-free,
  junk-free
from "02 Journal/Daily_Notes"
where contains(aliases, "dietlog")
sort file.day desc
```