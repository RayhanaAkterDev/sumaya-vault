---
exampleProperty: code
---
`INPUT[text:exampleProperty]`

```dataviewjs
const query = (dv.current().exampleProperty || "").toLowerCase().trim();

if (!query) {
  dv.paragraph("Start typing to search your notes...");
} else {
  const results = dv.pages().where(page => {
    const nameMatch = page.file.name.toLowerCase().includes(query);

    const tagList = Array.isArray(page.tags)
      ? page.tags
      : (typeof page.tags === "string" ? [page.tags] : []);
    const tagMatch = tagList.some(tag => tag.toLowerCase().includes(query));

    const yamlValues = Object.values(page)
      .filter(val => typeof val === "string" || Array.isArray(val))
      .flat()
      .map(val => val.toString().toLowerCase());

    const yamlMatch = yamlValues.some(val => val.includes(query));

    return nameMatch || tagMatch || yamlMatch;
  });

  const sorted = results.sort(p => p.file.ctime, 'asc');

  dv.table(
    ["File", "Tags", "Created", "Folder"],
    sorted.map(p => [
      dv.fileLink(p.file.path),
      Array.isArray(p.tags) ? p.tags.join(", ") : (p.tags ?? "—"),
      p.file.ctime.toLocaleString(),
      p.file.folder
    ])
  );
}
```
