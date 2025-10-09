---
class: journal
title: Weekly Schedule
aliases:
  - weekly note
important_links:
---

# Weekly Schedule

> [!multi-column]
> 
>> [!info]
>> ##### 🗓️ Timeline: <% moment(tp.file.title, "gggg-[W]ww").startOf('isoWeek').add(6, 'days').format("MMM DD") %> - <% moment(tp.file.title, "gggg-[W]ww").startOf('isoWeek').add(12, 'days').format("MMM DD") %>
>> [[02 Journal/Weekly_Journal/<%moment(tp.file.title, "gggg-[W]ww").subtract(1,'week').format("gggg-[W]ww")%>|↺ Previous Week]] | [[02 Journal/Weekly_Journal/<%moment(tp.file.title, "gggg-[W]ww").add(1,'week').format("gggg-[W]ww")%>|Next Week ↻]]
>
>> [!tip] Quick Buttons
>> `BUTTON[quick_note]` 
>>  `BUTTON[edit_weekly_temp]` 

 ```meta-bind-embed
 [[MetaBindEmbeds Spaces Buttons]]
 ```

---

## Weekly Goals

_A list of key objectives to focus on this week, guiding your priorities and progress._

1. _add goal_

---

### Daily Log 

A quick reference to each day’s journal note for the week, helping track daily activities and reflections.

| Day       | Note                                                                                                                    |
| --------- | ----------------------------------------------------------------------------------------------------------------------- |
| Sunday    | [[02 Journal/Daily_Notes/<% moment(tp.file.title,"gggg-[W]ww").startOf('week').add(0,'days').format("YYYY-MM-DD") %>]]  |
| Monday    | [[02 Journal/Daily_Notes/<% moment(tp.file.title,"gggg-[W]ww").startOf('week').add(1,'days').format("YYYY-MM-DD") %>]]  |
| Tuesday   | [[02 Journal/Daily_Notes/<% moment(tp.file.title,"gggg-[W]ww").startOf('week').add(2,'days').format("YYYY-MM-DD") %>]]  |
| Wednesday | [[02 Journal/Daily_Notes/<% moment(tp.file.title,"gggg-[W]ww").startOf('week').add(3,'days').format("YYYY-MM-DD") %>]]  |
| Thursday  | [[02 Journal/Daily_Notes/<% moment(tp.file.title,"gggg-[W]ww").startOf('week').add(4,'days').format("YYYY-MM-DD") %>]]  |
| Friday    | [[02 Journal/Daily_Notes/<% moment(tp.file.title,"gggg-[W]ww").startOf('week').add(5,'days').format("YYYY-MM-DD") %>]]  |
| Saturday  | [[02 Journal/Daily_Notes/<% moment(tp.file.title,"gggg-[W]ww").startOf('week').add(6,'days').format("YYYY-MM-DD") %>]]  |

---

### Calendar Overview

```dataview
CALENDAR date(file.name)
FROM "02 Journal/Daily_Notes"
```

---

## Weekly Reflection

- 🌟 Highlights of the Week
- ⚡ Challenges Faced
- 📌 Lessons Learned  

### Gratitude

- Things I’m grateful for this week:  

