# 🧱 GitHub Features

This section introduces essential **GitHub features** that help you collaborate, automate, and manage your projects effectively.

---

## 🔄 Pull Requests (PRs)

Pull Requests are the core of collaboration on GitHub.  
They let you review, discuss, and merge code changes.

| Command / Action | Description |
|------------------|-------------|
| Create PR | Compare branches and propose changes. |
| Review PR | Add comments, approve, or request modifications. |
| Merge PR | Integrate approved changes into the base branch. |
| Close PR | Discard changes without merging. |

**Steps to Create a Pull Request:**
1. Push your branch to GitHub.  
2. Open your repo on GitHub.  
3. Click **“Compare & Pull Request.”**  
4. Add a title and description.  
5. Submit for review.

---

## 🧩 Issues

GitHub Issues help you track bugs, tasks, and feature requests.

| Feature | Description |
|----------|-------------|
| Create Issue | Use templates or write a custom one. |
| Assign Labels | Categorize issues (bug, enhancement, etc.). |
| Link PRs | Connect PRs to issues for automatic closure. |
| Close Issue | Mark an issue as resolved. |

Example:
```
Fixes #21
```
(This closes issue #21 when merged.)

---

## ⚙️ GitHub Actions

GitHub Actions automate workflows like testing, deployment, or code formatting.

| File | Description |
|------|-------------|
| `.github/workflows/` | Folder containing workflow YAML files. |
| `main.yml` | Defines the workflow, triggers, and actions. |

Example:
```yaml
name: CI Pipeline
on: [push, pull_request]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Run Tests
        run: npm test
```

---

## 🍴 Forking Repositories

Forking lets you copy someone else’s repository into your account to make independent changes.

| Action | Description |
|---------|-------------|
| Fork | Creates a copy of another user’s repository. |
| Clone | Download the fork locally. |
| Pull Request | Submit your changes to the original repository. |

---

## ⭐ Starring and Watching

| Action | Description |
|----------|-------------|
| ⭐ Star | Save or bookmark repositories you like. |
| 👀 Watch | Get notifications for updates and activity. |

---

## 🧠 Discussions and Wikis

- **Discussions** – For community Q&A and brainstorming.  
- **Wiki** – To maintain detailed project documentation.

---

## 💡 Tip
Use **Issues + Pull Requests + Actions** to create a full DevOps workflow on GitHub.

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
