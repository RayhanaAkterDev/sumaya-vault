---
title: u-capture
---

```datacards
TABLE title, source, description
FROM "@u-capture"
where
  (
    length(split(file.folder, "/")) = length(split("@u-capture", "/"))
    or (
      length(split(file.folder, "/")) = length(split("@u-capture", "/")) + 1
      and contains(file.folder, file.name)
    ) 
  )

sort file.name asc

// Settings
preset: portrait
imageProperty: cover
```