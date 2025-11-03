# ⚙️ Advanced Git Concepts

This section explores **powerful Git commands and techniques** that help you handle complex version control workflows — including rebasing, stashing, cherry-picking, tagging, and resetting.

---

## 🔁 Rebasing

Rebasing helps maintain a **clean, linear project history**.

| Command | Description |
|----------|-------------|
| `git rebase <branch>` | Moves or combines a sequence of commits onto another branch. |
| `git rebase -i <commit>` | Interactive rebase — edit, squash, or reorder commits. |
| `git rebase --continue` | Continues after resolving rebase conflicts. |
| `git rebase --abort` | Cancels the rebase process. |

Example:
```bash
git checkout feature
git rebase main
```

---

## 🧳 Stashing Changes

Stash temporarily saves your local modifications without committing them.

| Command | Description |
|----------|-------------|
| `git stash` | Saves current uncommitted changes. |
| `git stash list` | Shows all stashed entries. |
| `git stash pop` | Applies the latest stash and removes it from the list. |
| `git stash apply` | Applies a stash but keeps it in the list. |
| `git stash drop` | Deletes a specific stash entry. |

Example:
```bash
git stash save "Work in progress"
git pull origin main
git stash pop
```

---

## 🍒 Cherry-Picking Commits

Cherry-picking lets you apply a specific commit from one branch to another.

| Command | Description |
|----------|-------------|
| `git cherry-pick <commit_hash>` | Applies the changes introduced by the specific commit. |

Example:
```bash
git checkout main
git cherry-pick a1b2c3d
```

---

## 🏷️ Tagging Versions

Tags mark specific points in history (often for releases).

| Command | Description |
|----------|-------------|
| `git tag` | Lists all tags. |
| `git tag <name>` | Creates a lightweight tag. |
| `git tag -a <name> -m "message"` | Creates an annotated tag with a message. |
| `git push origin --tags` | Pushes all tags to the remote repository. |

Example:
```bash
git tag -a v1.0 -m "First release"
git push origin v1.0
```

---

## 🧨 Resetting and Reverting

| Command | Description |
|----------|-------------|
| `git reset <file>` | Unstages a file. |
| `git reset --soft <commit>` | Moves HEAD to a previous commit but keeps changes staged. |
| `git reset --hard <commit>` | Discards all changes and resets to a specific commit. |
| `git revert <commit>` | Creates a new commit that undoes the specified commit safely. |

Example:
```bash
git reset --hard HEAD~1
```

---

## 💡 Tip
Use `rebase` for clean history, `merge` for preserving branches, and `stash` to multitask efficiently.

---

## 🧑‍💻 Author
**Aditya Jadhav**  
📧 [adi.jadhav@example.com](mailto:adi.jadhav@example.com)  
🌐 [GitHub Profile](https://github.com/AdiJadhav1608)

---

## ⭐ Contribute
Contributions, suggestions, and improvements are welcome!  
1. Fork this repository  
2. Create a new branch  
3. Commit your changes  
4. Submit a Pull Request  

---

⭐ *If you found this helpful, give it a star and keep exploring Git & GitHub!*
