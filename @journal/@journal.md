---
Title: Daily Note
---
[[+ About Journal ℹ️]]

# 🗂️ Journal Overview

_A quick-access dashboard of your monthly, weekly, and daily journal entries._


## 📅 Monthly View

```dataview
CALENDAR date(file.name)
FROM "@journal/Daily_Notes"
```
---

## 📒 Weekly Journal Entries

```dataview
list
FROM "@journal/Weekly_Journal"
SORT file.ctime DESC
```

---

## 📑 Daily Notes (List)

```dataview
list
FROM "@journal/Daily_Notes"
SORT file.name desc
```
