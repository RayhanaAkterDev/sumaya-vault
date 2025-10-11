---
fields:
  - name: title
    type: Input
    options:
      template: ""
    path: ""
    id: Mhjz44
  - name: course
    type: Select
    options:
      sourceType: ValuesList
      valuesList:
        "1": Computer Network
        "2": Software Engineering
        "3": Embedded System Programming
        "4": Theory of Computation
    path: ""
    id: VHgGdZ
  - name: chapter
    type: Select
    options:
      sourceType: ValuesList
      valuesList:
        "1": "ch1: {{chapter-name}}"
        "2": "ch2: {{chapter-name}}"
        "3": "ch3: {{chapter-name}}"
        "4": "ch4: {{chapter-name}}"
        "5": "ch5: {{chapter-name}}"
        "6": "ch6: {{chapter-name}}"
        "7": "ch7: {{chapter-name}}"
        "8": "ch8: {{chapter-name}}"
        "9": "ch9: {{chapter-name}}"
    path: ""
    id: ldreue
  - name: semester
    type: Select
    options:
      sourceType: ValuesList
      valuesList:
        "1": 1st
        "2": 2nd
        "3": 3rd
        "4": 4th
        "5": 5th
        "6": 6th
        "7": 7th
        "8": 8th
    path: ""
    id: NkaCEz
  - name: date
    type: Date
    options:
      dateShiftInterval: 1 day
      dateFormat: YYYY-MM-DD
      defaultInsertAsLink: false
      linkPath: ""
    path: ""
    id: A6bnAy
  - name: status
    type: Select
    options:
      sourceType: ValuesList
      valuesList:
        "1": todo 🔖
        "2": working 🚀
        "3": pending ⏳
        "4": done ✅
        "5": incomplete ⚠️
    path: ""
    id: T8dmGd
  - name: importance
    type: Select
    options:
      sourceType: ValuesList
      valuesList:
        "1": ⭐
        "2": ⭐⭐
        "3": ⭐⭐⭐
        "4": ⭐⭐⭐⭐
        "5": ⭐⭐⭐⭐⭐
    path: ""
    id: XzBrjk
  - name: Note
    type: Input
    options:
      template: Check / see exam kit page no. ...
    path: ""
    id: 1TKMmq
version: "2.43"
limit: 20
mapWithTag: false
icon: book-text
tagNames:
filesPaths:
bookmarksGroups:
excludes:
extends:
savedViews: []
favoriteView:
fieldsOrder:
  - 1TKMmq
  - XzBrjk
  - Mhjz44
  - VHgGdZ
  - ldreue
  - NkaCEz
  - A6bnAy
  - T8dmGd
---
