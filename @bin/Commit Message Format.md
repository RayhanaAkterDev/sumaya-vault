# 📌 Commit Message Format (Conventional + Folder Scoped)

## 🔹 Header (required)
<type>(<folder/subfolder>): <short summary in present tense>

### Examples:
feat(myfolio/about): add responsive About section layout  
chore(myfolio/setup): initialize folder structure  
fix(css/box-model): resolve padding overflow issue on mobile  

---

## 🔹 Body (optional but recommended)
Explain the "what" and "why" in full sentences.  
Use this to give extra context, describe changes in detail, or list added files.

### Example:
Add a new "About" section using flexbox for layout.  
Include responsive design and styling for different screen sizes.  
Imported an avatar image and wrote descriptive text.

---

## 🔹 Common Commit Types
| Type     | Meaning                                       |
|----------|-----------------------------------------------|
| feat     | New feature or section                        |
| fix      | Bug fix or layout issue                       |
| chore    | Setup, folder structure, configs              |
| style    | CSS-only changes, no logic                    |
| refactor | Code rewrite without new feature or fix       |
| docs     | Documentation or README updates               |
| test     | Adding or updating tests                      |

---

## 🛠 Recommended Commit Flow
1. Make your changes
2. Stage files with `git add .`
3. Commit using this format
4. Push with `git push`

