---
limit: 20
mapWithTag: false
icon: pen
tagNames: 
filesPaths: 
bookmarksGroups: 
excludes: 
extends: 
savedViews: []
favoriteView: 
fieldsOrder:
  - x5eGwf
  - 0CW2Kh
  - TphyZV
version: "2.9"
fields:
  - name: title
    type: Input
    options: {}
    path: ""
    id: x5eGwf  
  - name: date
    type: DateTime
    options:
      dateShiftInterval: 1 day
      dateFormat: YYYY-MM-DD hh:mm a
      defaultInsertAsLink: false
      linkPath: ""
    path: ""
    id: 0CW2Kh
  - name: status
    type: Select
    options:
      sourceType: ValuesList
      valuesList:
        "1": In Progress
        "2": Pending
        "3": Done
    path: ""
    id: TphyZV
---