# 🌐 Remote Operations in Git

This section covers how to work with **remote repositories** — including cloning, pushing, pulling, and synchronizing your work with platforms like GitHub.

---

## 🔗 Working with Remotes

| Command | Description |
|----------|-------------|
| `git remote -v` | Lists all configured remote repositories. |
| `git remote add origin <url>` | Adds a remote repository connection. |
| `git remote remove <name>` | Removes a remote. |
| `git remote rename <old> <new>` | Renames a remote. |

---

## 📥 Cloning a Repository

| Command | Description |
|----------|-------------|
| `git clone <url>` | Creates a local copy of a remote repository. |
| `git clone <url> <folder>` | Clones into a specific folder. |

Example:
```bash
git clone https://github.com/AdiJadhav1608/Git-GitHub-Guide.git
```

---

## 📤 Pushing Changes to Remote

| Command | Description |
|----------|-------------|
| `git push origin main` | Pushes local changes to the `main` branch on the remote. |
| `git push -u origin main` | Sets upstream for future pushes. |
| `git push origin <branch>` | Pushes a specific branch. |
| `git push --all` | Pushes all local branches. |
| `git push --tags` | Pushes all tags to the remote. |

---

## 📥 Pulling and Fetching Changes

| Command | Description |
|----------|-------------|
| `git fetch` | Retrieves updates from remote but doesn’t merge. |
| `git pull` | Fetches and merges updates into your local branch. |
| `git pull origin main` | Pulls the latest changes from `main` branch. |

---

## 🔄 Synchronizing Forks

If you forked a repository, keep it updated using:
```bash
git remote add upstream <original_repo_url>
git fetch upstream
git merge upstream/main
```

---

## 🧩 Removing Remote Tracking Branches

| Command | Description |
|----------|-------------|
| `git remote prune origin` | Removes outdated references to deleted branches. |
| `git fetch -p` | Prunes while fetching updates. |

---

## 💡 Tip
Always **pull before you push** to avoid merge conflicts.

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
