---
searchTerm: ""
---
## Search Box

```meta-bind
INPUT[text:searchTerm]
```

---

### Dataview Query for Notes

```dataview
TABLE WITHOUT ID
	file.link as session, 
	created, 
	tags
FROM !"10 Templates"
WHERE this.searchTerm != null
AND this.searchTerm != ""
AND all(split(this.searchTerm, " "), (term) =>(
	icontains(tags, term) OR
	icontains(lower(file.name), term)
))
SORT filename DESC
```

---

###  Dataview Query for Logs

```dataview
TASK
WHERE this.searchTerm != null
AND this.searchTerm != ""
AND all(split(this.searchTerm, " "), (term) => icontains(text, term))
GROUP BY file.name as filename
SORT filename DESC
```