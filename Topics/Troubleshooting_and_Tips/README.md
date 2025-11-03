# 🛠️ Troubleshooting and Tips

This section provides common **Git & GitHub errors**, their **solutions**, and **pro tips** to improve your workflow efficiency.

---

## ⚠️ Common Git Errors and Fixes

### ❌ Error: `fatal: not a git repository`
**Cause:** You’re not inside a Git-initialized folder.  
**Fix:**
```bash
cd project-folder
git init
```

---

### 🔐 Error: `Authentication failed`
**Cause:** GitHub removed password authentication.  
**Fix:**
Use a **Personal Access Token (PAT)** instead of a password.

```bash
git remote set-url origin https://<username>:<TOKEN>@github.com/<username>/<repo>.git
```

---

### 🔄 Error: `failed to push some refs`
**Cause:** Remote branch has new commits you don’t have locally.  
**Fix:**
```bash
git pull origin main --rebase
git push origin main
```

---

### ⚙️ Error: `merge conflicts`
**Cause:** Changes in the same file differ between branches.  
**Fix:**
1. Open the conflicting file.  
2. Manually resolve conflicts.  
3. Stage and commit the resolved file.  

```bash
git add <filename>
git commit -m "Resolved merge conflict"
```

---

### 🧩 Error: `src refspec main does not match any`
**Cause:** The branch name is wrong or no commits exist yet.  
**Fix:**
```bash
git branch -M main
git add .
git commit -m "Initial commit"
git push -u origin main
```

---

## 💡 Pro Tips for Git & GitHub

| Tip | Description |
|-----|-------------|
| ✅ Use `.gitignore` | Exclude unnecessary files from your repo. |
| 🪄 Use `git status` often | Check your repo state before committing. |
| 🧹 Clean history | Use `git rebase -i` for neat commit logs. |
| 🚀 Automate | Use GitHub Actions for CI/CD workflows. |
| 🔒 Security | Never push secrets or credentials to GitHub. |
| 🧠 Learn branching | Follow Git Flow or Trunk-Based branching. |

---

## 🪶 Useful Commands Reference

```bash
# Undo last commit (keep changes)
git reset --soft HEAD~1

# Undo last commit (discard changes)
git reset --hard HEAD~1

# See all branches
git branch -a

# Delete local branch
git branch -d branch-name

# Delete remote branch
git push origin --delete branch-name

# View commit history
git log --oneline --graph --decorate
```

---

## 🔧 Recommended Extensions for VS Code

| Extension | Description |
|------------|-------------|
| GitLens | Visualize Git history and blame info. |
| GitHub Pull Requests | Manage PRs directly in VS Code. |
| Code Spell Checker | Prevent typos in commits. |
| Markdown All in One | Format and preview your README easily. |

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

⭐ *If you found this helpful, give it a star and keep mastering Git & GitHub!*
