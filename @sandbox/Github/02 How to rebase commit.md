1. `git rebase -i HEAD~N`
2. `n`
3. `rm -rf .git/rebase-merge`
4. `git push --force`

---

**how to rebase/edit the last commit that already pushed**

- `git commit --amend`
- `git push --force`

---

**✅ To remove the last commit (if not pushed yet):**

- `git reset --hard HEAD~1`

---

**⚠️ If you want to keep the changes but just undo the commit:**

- Undo the last commit but keep all changes staged - `git reset --soft HEAD~1`
- Unstage all files - `git reset`
- Stage only the specific file/folder -  `git add file/folder-path`
- Commit only that file/folder - `git commit -m "commit-msg"`
- ✅ You're now ready to push - `git push`

---