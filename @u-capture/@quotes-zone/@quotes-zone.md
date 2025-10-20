---
title: Quotes Zone
tags: quote
---

```datacards
TABLE cover, title
FROM "@u-capture/@quotes-zone"
WHERE file.name != "@u-capture/@quotes-zone"
	AND file.name != "@quotes-zone"

// Settings
preset: portrait
imageProperty: cover
```