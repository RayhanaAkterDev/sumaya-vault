---
title: How to commit?
class: note
date: 2025-10-03 09:35 pm
tags:
  - code
  - git-github
---


# ✅ How to Write Good Commit Messages (Professional Approach)

To maintain clarity and consistency — especially when building a portfolio or working in teams — follow the **Conventional Commit** style:

## 🔧 Commit Message Format:

```cpp
type(scope): message
```

---

## 🔑 Common Commit Types:

- `feat` – for adding a new feature    
- `fix` – for bug fixes    
- `docs` – for documentation changes (including comments inside code)    
- `style` – for formatting (white-space, missing semicolons, etc.)    
- `refactor` – for code changes that neither fix a bug nor add a feature    
- `test` – for adding or updating tests    
- `chore` – for routine tasks like config updates, package installs, etc.

### 📌 Special Clarification:

> - Use `docs` even inside `.html`, `.css`, or `.js` files **if you're only adding or editing comments** (non-functional).  
> - Use `feat`, `fix`, etc., when you're making changes to actual code or markup.
> - Use `refactor` when you **clean up or improve code structure** without changing its behavior (e.g., renaming variables, removing repetition).
> - Use `test` when you're **adding or modifying test cases** (e.g., unit tests, manual test instructions) — not actual code functionality.

---

## ✅ Examples:

| Situation                                          | Correct Commit                                               |
| -------------------------------------------------- | ------------------------------------------------------------ |
| Adding new form elements in HTML                   | `feat(html): add 06-forms.html with basic form structure`    |
| Adding comments inside HTML file to explain inputs | `docs(html): add comments for input fields in 06-forms.html` |
| Writing markdown notes about forms in README       | `docs(html-css): add form section to README.md`              |

### ✅ Example Commit Messages:

- `feat(html): add typography.html for text and heading tags`    
- `style(css): improve spacing and font styles in typography.css`    
- `docs(html-css): add README with topic overview and folder structure`    
- `refactor(responsive-design): optimize flexbox layout for mobile`    

---
## 🤝 Best Practices:

- Use **present tense**: “add”, not “added” or “adds”    
- Keep it **short and meaningful**    
- Group changes under one commit per logical task    
- Avoid mixing unrelated changes in one commit    
- Prefer clarity over creativity in professional repos

---

### ❌ Bad example (multi-topic commit — not ideal):

```bash
docs(html-css): add new form layout and fix font size in typography.css
```

🔎 This mixes two unrelated tasks:

- Adding a new layout (a feature)    
- Fixing font size (a bugfix or styling tweak)

### ✅ Good example (separated logical commits):

```bash
docs(html-css/forms)[html-css/forms] feat: add new form layout structure  
[html-css/css] fix: correct font size in typography.css
```

Now each commit is focused and clear.

---

> This approach improves collaboration, allows better changelogs, and signals professionalism to recruiters and team leads.