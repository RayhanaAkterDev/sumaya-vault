```dataview
table 
  tahajjut, 
  fajr, 
  dhuhr, 
  asr, 
  maghrib, 
  isha, 
  join(map(split(kaja, ","), (x) => "• " + x), "<br>") as kaja
from "02 Journal/Daily_Notes"
where contains(aliases, "salat_record")
sort file.day desc
```