---
exampleProperty: ""
---
`INPUT[text:exampleProperty]`

```dataviewjs
const search = (dv.current().exampleProperty || "").toLowerCase();

const pages = dv.pages().where(p => {
    const nameMatch = p.file.name.toLowerCase().includes(search);

    // Handle YAML tags
    const rawTags = p.tags ?? [];
    const tags = Array.isArray(rawTags)
        ? rawTags
        : (typeof rawTags === "string" ? [rawTags] : []);
    const tagMatch = tags.some(tag => tag.toLowerCase().includes(search));

    // Search in YAML fields like title, status, etc.
    const yamlValues = Object.values(p)
        .filter(val => typeof val === "string" || Array.isArray(val))
        .flat()
        .map(val => val.toString().toLowerCase());

    const yamlMatch = yamlValues.some(val => val.includes(search));

    return search !== "" && (nameMatch || tagMatch || yamlMatch);
});

// Sort by created date (optional)
const sortedPages = pages.sort(p => p.file.ctime, 'asc');

// Build table
dv.table(
    ["File", "Tags", "Created", "Parent Folder"],
    sortedPages.map(p => [
        dv.fileLink(p.file.path),
        (Array.isArray(p.tags) ? p.tags.join(", ") : p.tags ?? "—"),
        p.file.ctime.toLocaleString(),
        p.file.folder
    ])
);
```
