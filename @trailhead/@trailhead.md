```dataview
table dateformat(file.ctime, "yyyy-MM-dd") as "Created",  file.mtime as "Modified"
from "16 DataViews"
where length(split(file.folder, "/")) <= 2
sort file.name
```

---

 `BUTTON[new_note]` 

 ```meta-bind-embed
 [[MetaBindEmbeds Spaces Buttons]]
 ```


