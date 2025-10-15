---
title: Journal Note
class: journal
---
[[+ About Journal ℹ️]]

# 🗂️ Journal Overview

_A quick-access dashboard of your monthly, weekly, and daily journal entries._


## 📅 Monthly View

```dataview
CALENDAR date(file.name)
FROM "@journal/@daily-notes"
```
---

## 📒 Weekly Journal Entries

```dataview
list
FROM "@journal/@weekly-notes"
SORT file.ctime DESC
```

---

## 📑 Daily Notes (List)

```dataview
list
FROM "@journal/@daily-notes"
SORT file.name desc
```
