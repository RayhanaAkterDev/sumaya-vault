---
class: note
title: MetaBindEmbeds Spaces Buttons
date: 2025-07-28 07:56 pm
status: Done
---

```meta-bind-button
label: New note
icon: plus
style: primary
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: Create a new file
id: new_note
hidden: true
actions:
  - type: command
    command: file-explorer:new-file
```

```meta-bind-button
label: Open Vault 🗃️
icon: ""
style: default
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: openvault
hidden: true
actions:
  - type: open
    link: "[[00 MOCs]]"
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
id: edit_daily_temp
hidden: true
actions:
  - type: open
    link: "[[10 Templates/daily_template]]"
    newTab: true
```

```meta-bind-button
label: 🖋️ Edit Template
icon: ""
style: default
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: edit_fleeting_note_temp
hidden: true
actions:
  - type: open
    link: "[[10 Templates/fleeting_note_template]]"
    newTab: true
```

```meta-bind-button
label: Reload 🔄
icon: ""
style: primary
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: reload
hidden: true
actions:
  - type: command
    command: app:reload
```

```meta-bind-button
label: 🏠 Home
icon: ""
style: primary
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: "HOME"
hidden: true
actions:
  - type: command
    command: workspace:goto-tab-1
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
    link: "[[10 Templates/weekly_template]]"
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
    link: "[[10 Templates/discovery_log]]"
    newTab: true
```