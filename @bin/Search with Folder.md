---
exampleProperty: "#code"
searchFolder: '"02 Journal"'
---

## Select Folder

```meta-bind
INPUT[select(
  option("Select Folder"),
  option("01 NoteLab"),
  option("02 Journal"),
  option("03 Self Discipline"),
  option("06 CSE DIIT")
):searchFolder]
```

---

## Search Box

`INPUT[text:exampleProperty]`

---

```dataviewjs
const folder = dv.current().searchFolder?.trim();
const term = dv.current().exampleProperty?.toLowerCase().trim();

dv.paragraph(`📂 Folder: "${folder}"`);
dv.paragraph(`🔍 Term: "${term}"`);

if (folder && term) {
  // Search pages in the folder whose filename contains the term (case-insensitive)
  const results = dv.pages(folder)
    .where(p => p.file.name.toLowerCase().includes(term))
    .sort(p => p.file.name, 'asc');

  if (results.length > 0) {
    // Create a table with the desired columns
    dv.table(
      ["File", "Parent Folder", "Tags", "Course", "Semester", "Chapter"],
      results.map(p => [
        dv.fileLink(p.file.path, false),
        p.file.folder,
        p.tags ? p.tags.join(", ") : "",
        p.course ?? "",
        p.semester ?? "",
        Array.isArray(p.chapter) ? p.chapter.join(", ") : (p.chapter ?? "")
      ])
    );
  } else {
    dv.paragraph("❌ No matching files.");
  }
} else {
  dv.paragraph("⚠️ Please select folder and enter search term.");
}
```