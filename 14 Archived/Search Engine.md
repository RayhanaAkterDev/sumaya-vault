---
Title: Search Engine
searchTerm: code
---

## Search Vault

```meta-bind
INPUT[text:searchTerm]
```

### Results: Notes

```dataviewjs
const input = (dv.current().searchTerm || "").trim().toLowerCase();

if (!input) {
  dv.paragraph("Nothing to show — start searching in the search box to see results.");
} else {
  const results = dv.pages()
    .where(p => !p.file.folder.startsWith("10 Templates"))
    .where(p => {
      const nameMatch = p.file.name.toLowerCase().includes(input);
      const tagList = Array.isArray(p.file.tags)
        ? p.file.tags.map(t => t.toLowerCase())
        : (typeof p.file.tags === "string" ? [p.file.tags.toLowerCase()] : []);
      const tagMatch = tagList.some(t => t.includes(input));
      return nameMatch || tagMatch;
    })
    .sort(p => p.file.name, 'desc');

  dv.table(
    ["File", "Tags"],
    results.map(p => [
      dv.fileLink(p.file.path),
      dv.el("ul",
        (Array.isArray(p.file.tags)
          ? p.file.tags
          : (typeof p.file.tags === "string" ? [p.file.tags] : [])
        ).map(tag => dv.el("li", tag))
      )
    ])
  );
}
```

---

### Results: Tasks

```dataviewjs
const input = (dv.current().searchTerm || "").trim().toLowerCase();

if (!input) {
  dv.paragraph("Nothing to show — start searching in the search box to see results.");
} else {
  // Get all tasks in all pages except "10 Templates" folder
  const tasks = dv.pages()
    .where(p => !p.file.folder.startsWith("10 Templates"))
    .file
    .tasks
    .where(t => !t.completed);

  // Group by file path
  const taskMap = new Map();

  for (const task of tasks) {
    const path = task.path;
    const fileName = path.split("/").pop().toLowerCase();

    const tags = Array.isArray(task.tags)
      ? task.tags.map(t => t.toLowerCase())
      : [];

    const matches =
      task.text.toLowerCase().includes(input) ||
      fileName.includes(input) ||
      tags.some(tag => tag.includes(input));

    if (!matches) continue;

    if (!taskMap.has(path)) {
      taskMap.set(path, []);
    }

    taskMap.get(path).push(task);
  }

  if (taskMap.size === 0) {
    dv.paragraph("No matching items found — try a different search term.");
  } else {
    // Render grouped tasks WITHOUT redundant file heading
    for (const [path, tasks] of taskMap.entries()) {
      // Remove this heading line if tasks show file heading themselves
      // dv.header(3, dv.fileLink(path));
      
      // Instead, just show tasks directly
      dv.taskList(tasks.sort((a, b) => a.line - b.line));
    }
  }
}
```