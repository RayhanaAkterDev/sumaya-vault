```dataviewjs
let pages = dv.pages()
  .where(p => p.aliases && p.aliases.includes("code_log") && p.file.name !== "daily_template")
  .sort(p => p.file.name, "desc");

if (!pages || pages.length === 0) {
  dv.paragraph("⚠️ No code_log pages found. Check aliases/YAML and save notes.");
} else {
  for (let p of pages) {
    dv.header(4, p.file.link);

    if (p.code_topics && Array.isArray(p.code_topics) && p.code_topics.length) {
      let md = "";
      for (let t of p.code_topics) {
        md += `- **${t.topic}**\n`;
        if (Array.isArray(t.items)) {
          for (let it of t.items) md += `  - ${it}\n`;
        } else if (t.items) {
          md += `  - ${t.items}\n`;
        }
      }

      // Render list as paragraph (safe) without extra trailing newline
      dv.paragraph(md.trim());
    } else {
      dv.paragraph("_No topics found_");
    }

    // ✅ Use Obsidian-native HR separator
    dv.paragraph('---');
  }
}
```
