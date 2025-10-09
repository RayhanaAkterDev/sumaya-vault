---
Title: Daily Note
aliases:
  - Journals
  - Journal Overview
---
[[+ About Journal ℹ️]]

# 🗂️ Journal Overview

_A quick-access dashboard of your monthly, weekly, and daily journal entries._

---

## 📅 Calendar View

```dataview
CALENDAR date(file.name)
FROM "02 Journal/Daily_Notes"
```

---

## 📆 Monthly Schedules

```dataview
TABLE file.folder AS Folder, dateformat(file.ctime, "yyyy-MM-dd") AS Created
FROM "02 Journal/Monthly_Schedule"
SORT file.ctime DESC
```

---

## 📒 Weekly Journal Entries

```dataview
TABLE file.folder AS Folder, dateformat(file.ctime, "yyyy-MM-dd") AS Created
FROM "02 Journal/Weekly_Journal"
SORT file.ctime DESC
```

---

## 📑 Daily Notes (Table View)

```dataview
TABLE file.folder AS Folder, dateformat(file.ctime, "yyyy-MM-dd") AS Created
FROM "02 Journal/Daily_Notes"
SORT file.name desc
```
