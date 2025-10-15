---
class: note
title: MetaBindEmbeds Spaces Buttons
date: 2025-07-28 07:56 pm
---

```meta-bind-button
label: 🖋️ Edit Template
icon: ""
style: primary
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: edit_daily_temp
hidden: true
actions:
  - type: open
    link: "[[01 Daily Note Template]]"
    newTab: true
```

```meta-bind-button
label: 🖋️ Edit Template
icon: ""
style: primary
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: edit_weekly_temp
hidden: true
actions:
  - type: open
    link: "[[02 Weekly Template]]"
    newTab: true
```

```meta-bind-button
label: 🖋️ Edit Template
icon: ""
style: primary
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: discovery_log
hidden: true
actions:
  - type: open
    link: "[[06 Resource Template]]"
    newTab: true
```

```meta-bind-button
label: Quick Note 📝
icon: ""
style: primary
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: quick_note
hidden: true
actions:
  - type: templaterCreateNote
    templateFile: 10 Templates/fleeting_note_template.md
    folderPath: 01 NoteLab
    fileName: New note
    openNote: false
    openIfAlreadyExists: true
  - type: open
    link: "[[New note]]"
    newTab: true

```

```meta-bind-button
 label: 👉 List View
 icon: ""
 style: default
 class: ""
 cssStyle: ""
 backgroundImage: ""
 tooltip: Open list view in new tab
 id: CN_List_View
 hidden: true
 actions:
   - type: open
     link: "[[List View]]"
     newTab: true
```

```meta-bind-button
 label: 👉 List View
 icon: ""
 style: default
 class: ""
 cssStyle: ""
 backgroundImage: ""
 tooltip: Open list view in new tab
 id: SE_List_View
 hidden: true
 actions:
   - type: open
     link: "[[List View]]"
     newTab: true
```