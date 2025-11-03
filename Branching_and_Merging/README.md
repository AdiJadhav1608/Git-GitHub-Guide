# 🌿 Branching and Merging in Git

This section explains how to create, manage, and merge branches in Git — allowing multiple versions of a project to be developed simultaneously.

---

## 🌱 Creating and Managing Branches

| Command | Description |
|----------|-------------|
| `git branch` | Lists all local branches. |
| `git branch <name>` | Creates a new branch. |
| `git checkout <branch>` | Switches to the specified branch. |
| `git checkout -b <branch>` | Creates and switches to a new branch. |
| `git branch -d <branch>` | Deletes a local branch safely. |
| `git branch -D <branch>` | Force deletes a local branch. |
| `git branch -m <old> <new>` | Renames a branch. |

---

## 🧭 Viewing Branches and Status

| Command | Description |
|----------|-------------|
| `git branch -v` | Shows the latest commit on each branch. |
| `git branch --merged` | Lists branches already merged into the current one. |
| `git branch --no-merged` | Lists branches not yet merged. |

---

## 🔀 Merging Branches

| Command | Description |
|----------|-------------|
| `git merge <branch>` | Merges the specified branch into the current one. |
| `git merge --no-ff <branch>` | Forces a merge commit (preserves history). |
| `git merge --abort` | Aborts a merge if conflicts occur. |

---

## ⚔️ Handling Merge Conflicts

When two branches modify the same part of a file, Git will mark it as a **conflict**.

1. Open the conflicting file(s).  
2. Look for conflict markers like:
   ```
   <<<<<<< HEAD
   your changes
   =======
   incoming changes
   >>>>>>> branch-name
   ```
3. Edit and remove the markers.  
4. Stage and commit the resolved files:
   ```bash
   git add .
   git commit -m "Resolved merge conflicts"
   ```

---

## 🌳 Viewing Branch History

| Command | Description |
|----------|-------------|
| `git log --oneline --graph --all` | Shows a visual graph of branches and commits. |
| `git show-branch` | Displays branches and their commits. |

---

## 💡 Tip
Use feature branches for new work — this keeps the `main` branch clean and production-ready.

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
