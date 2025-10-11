---
title: Connect a Local Folder to Remote GitHub Repository
class: note
date: 2025-10-09
tags:
  - code
  - git-github
---
# How to Connect a Local Folder to a Remote GitHub Repository

This note explains how to link a local folder to a GitHub repository and push your files safely.

---

## 1. Initialize a local Git repository
Open your terminal in the project folder:

```bash
git init
```

---

## 2. Add all files
Add all your project files to Git:

```bash
git add .
```

---

## 3. Commit the files
Create the first commit:

```bash
git commit -m "Initial commit"
```

---

## 4. Add the remote repository
Replace the URL with your GitHub repo SSH or HTTPS link:

```bash
git remote add origin git@github.com:USERNAME/REPO-NAME.git
```

Or, if using HTTPS:

```bash
git remote add origin https://github.com/USERNAME/REPO-NAME.git
```

---

## 5. Push the files
If your GitHub repo is empty:

```bash
git branch -M main
git push -u origin main
```

If the remote already has commits (e.g., README.md):

```bash
git pull origin main --allow-unrelated-histories
git push -u origin main
```

> ⚠️ If you want to overwrite remote completely, use:

```bash
git push -u origin main --force
```

---

## 6. Ignore local-only files
Add a `.gitignore` to avoid pushing local config or plugins.  
For Obsidian, use:

```gitignore
.obsidian/plugins/
.obsidian/workspace.json
.obsidian/appearance.json
.obsidian/snippets/
.DS_Store
Thumbs.db
desktop.ini
*.tmp
*.bak
*.swp
*.swo
```

---

## ✅ Tips
- Use `git status` often to see tracked/untracked changes.
- Close Obsidian or editors when performing Git operations to avoid locked files.
- Always commit `.gitignore` before pushing to prevent plugin/config files from causing errors.
