# 🚀 Git & GitHub Complete Learning Guide
*My Beginner-Friendly Documentation*

---

## 📌 Table of Contents

1. [Introduction](#introduction)
2. [What is Git?](#what-is-git)
3. [What is GitHub?](#what-is-github)
4. [Git vs GitHub](#git-vs-github)
5. [Git Installation](#git-installation)
6. [Initial Git Setup](#initial-git-setup)
7. [Git Repository & `git init`](#git-repository--git-init)
8. [Working Directory, Staging & Commit](#working-directory-staging--commit)
9. [Basic Git Commands](#basic-git-commands)
10. [Branching & Merging](#branching--merging)
11. [Remote Repositories](#remote-repositories)
12. [Sharing & Updating Code](#sharing--updating-code)
13. [Tracking File Changes](#tracking-file-changes)
14. [Temporary Commits (Stash)](#temporary-commits-stash)
15. [Rewriting History](#rewriting-history)
16. [Inspecting & Comparing](#inspecting--comparing)
17. [Ignoring Files (`.gitignore`)](#ignoring-files-gitignore)
18. [Best Practices](#best-practices)
19. [Conclusion](#conclusion)

---

## 📘 Introduction

This document is a **complete Git & GitHub learning guide** created from the official **GitHub Education Git Sheet** and expanded with **clear explanations**, **real-world usage**, and **professional standards**.
 
**Perfect for:**
- 🚀 Beginners
- 🎓 Students
- 💻 Junior Developers
- 🏢 Professional Teams

---

## 🔧 What is Git?

**Git** is a **free and open-source distributed version control system**.

### 🔹 Why Git?

- ✅ Tracks code changes
- ✅ Maintains history
- ✅ Enables team collaboration
- ✅ Prevents code loss
- ✅ Allows rollback to previous versions

📌 **Git works locally on your computer.**

---

## 🌐 What is GitHub?

**GitHub** is a **cloud-based platform** that hosts Git repositories.

### 🔹 Why GitHub?

- ☁️ Store code online
- 👥 Collaborate with teams
- 🌍 Share projects
- 🎯 Manage issues & pull requests
- 🤖 CI/CD & automation

📌 **GitHub uses Git internally.**

---

## ⚖️ Git vs GitHub

| **Git** | **GitHub** |
|---------|-----------|
| Local tool | Online platform |
| Version control | Code hosting |
| Works offline | Requires internet |
| CLI based | Web + GUI |

---

## 💻 Git Installation

Download Git from the official site:

🔗 [https://git-scm.com](https://git-scm.com)

### GitHub Desktop (Optional GUI)

- **Windows:** [https://windows.github.com](https://windows.github.com)
- **Mac:** [https://mac.github.com](https://mac.github.com)

---

## ⚙️ Initial Git Setup

Configure your identity **(required)**:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

Enable colored output:

```bash
git config --global color.ui auto
```

---

## 📁 Git Repository & `git init`

### 🔹 What is a Repository?

A Git repository is a folder where Git tracks all changes.

### 🔹 `git init` Definition

```bash
git init
```

**Initializes a directory as a Git repository.**

It creates a hidden `.git` folder that stores:
- Commit history
- Branches
- Configuration

📌 **Use this when starting a new project.**

---

## 📂 Working Directory, Staging & Commit

Git has **3 stages**:

1. **Working Directory** – where you edit files
2. **Staging Area** – files ready for commit
3. **Repository** – committed snapshots

---

## 🧩 Basic Git Commands

### Check status

```bash
git status
```

Shows modified, staged, and untracked files.

### Stage a file

```bash
git add file_name
```

Adds file to the staging area.

### Unstage a file

```bash
git reset file_name
```

Removes file from staging but keeps changes.

### View changes

```bash
git diff
```

Shows unstaged changes.

```bash
git diff --staged
```

Shows staged changes.

### Commit changes

```bash
git commit -m "Descriptive commit message"
```

Creates a snapshot of staged files.

---

## 🌿 Branching & Merging

### List branches

```bash
git branch
```

### Create a new branch

```bash
git branch branch_name
```

### Switch branch

```bash
git checkout branch_name
```

### Merge branch

```bash
git merge branch_name
```

📌 **Branches allow parallel development.**

---

## 🌍 Remote Repositories

### Clone a repository

```bash
git clone repository_url
```

### Add remote

```bash
git remote add origin repository_url
```

---

## 🔄 Sharing & Updating Code

### Fetch updates

```bash
git fetch origin
```

### Pull updates

```bash
git pull
```

### Push changes

```bash
git push origin branch_name
```

---

## 🗂️ Tracking File Changes

### Remove file

```bash
git rm file_name
```

### Rename or move file

```bash
git mv old_path new_path
```

### View movement history

```bash
git log --stat -M
```

---

## 📦 Temporary Commits (Stash)

### Save changes temporarily

```bash
git stash
```

### View stash list

```bash
git stash list
```

### Apply stash

```bash
git stash pop
```

### Remove stash

```bash
git stash drop
```

📌 **Useful when switching branches mid-work.**

---

## ✍️ Rewriting History

### Rebase branch

```bash
git rebase branch_name
```

### Hard reset

```bash
git reset --hard commit_hash
```

⚠️ **Use carefully – may delete history.**

---

## 🔍 Inspecting & Comparing

### View commit history

```bash
git log
```

### Compare branches

```bash
git diff branchB...branchA
```

### Show commit details

```bash
git show commit_hash
```

---

## 🚫 Ignoring Files (`.gitignore`)

### Global ignore

```bash
git config --global core.excludesfile ~/.gitignore
```

### Example `.gitignore`

```
logs/
*.notes
node_modules/
.env
```

📌 **Prevents unnecessary files from being committed.**

---

## ✅ Best Practices

- ✔ Write meaningful commit messages
- ✔ Commit small changes
- ✔ Use branches
- ✔ Pull before push
- ✔ Never commit secrets
- ✔ Use `.gitignore`

---

## 🎯 Conclusion

This document provides a **complete, professional, and structured guide** to learning Git & GitHub from scratch to advanced usage.

📌 **Mastering Git is essential for:**

- 💼 Software Engineers
- 🌟 Open Source Contributors
- 👨‍💻 Professional Developers

---

**Happy Coding! 🚀**