---
title: button plugin
---

_New Note:_	
```button
name New note
type command
action Create new note
color blue
```
^button-note

---

_New prompt:_

```button
name Add new prompt
type note(@prompt no. — {{prompt}}, tab) template
action 05 Prompt Template
color purple
folder @u-capture/@prompts
prompt true
```
^button-prompt

---

_resource button:_

```button
name Add resource
type note(Resource, tab) template
action 06 Resource Template
color blue
folder @u-capture/@resources
prompt true
```
^button-resource

---

_quote button:_

```button
name Add new quote
type note({{quote}}, tab) template
action 07 Quote Template
color yellow
folder @u-capture/@quotes-zone
prompt true
```
^button-quote

---

_capture button:_

```button
name Insert new capture
type command
action Unique note creator: Create new unique note
color green
```
^button-capture