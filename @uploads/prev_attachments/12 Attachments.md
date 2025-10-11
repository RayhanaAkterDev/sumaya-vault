```dataview
table file.folder as "Folder", dateformat(file.ctime, "yyyy-MM-dd") as "Created"
from "12 Attachments"
where length(split(file.folder, "/")) = 1
  and contains(file.path, file.folder + "/" + file.folder + ".md")
sort file.name asc
```
