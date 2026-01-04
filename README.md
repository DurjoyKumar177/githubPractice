# 🚀 Git & GitHub Complete Learning Guide

*My Beginner-Friendly Documentation*

---

> **📥 Download PDF Version:** [Click here to download](./git_note_with_command.pdf)

---

## 📌 Table of Contents

1. [Introduction](#-introduction)
2. [What is Git?](#-what-is-git)
3. [What is GitHub?](#-what-is-github)
4. [Git vs GitHub](#️-git-vs-github)
5. [Git Installation](#-git-installation)
6. [Initial Git Setup](#️-initial-git-setup)
7. [Git Repository & git init](#-git-repository--git-init)
8. [Working Directory, Staging & Commit](#-working-directory-staging--commit)
9. [Basic Git Commands](#-basic-git-commands)
10. [Branching & Merging](#-branching--merging)
11. [Remote Repositories](#-remote-repositories)
12. [Sharing & Updating Code](#-sharing--updating-code)
13. [Tracking File Changes](#️-tracking-file-changes)
14. [Temporary Commits (Stash)](#-temporary-commits-stash)
15. [Rewriting History](#️-rewriting-history)
16. [Inspecting & Comparing](#-inspecting--comparing)
17. [Ignoring Files (.gitignore)](#-ignoring-files-gitignore)
18. [Best Practices](#-best-practices)
19. [Conclusion](#-conclusion)

---

## 📘 Introduction

This document is a **complete Git & GitHub learning guide** created from the official **GitHub Education Git Sheet** and expanded with **clear explanations**, **real-world usage**, and **professional standards**.
 
**Perfect for:**
- 🚀 Beginners
- 🎓 Students
- 💻 Junior Developers
- 🏢 Professional Teams

[⬆️ Back to Table of Contents](#-table-of-contents)

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

[⬆️ Back to Table of Contents](#-table-of-contents)

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

[⬆️ Back to Table of Contents](#-table-of-contents)

---

## ⚖️ Git vs GitHub

| **Git** | **GitHub** |
|---------|-----------|
| Local tool | Online platform |
| Version control | Code hosting |
| Works offline | Requires internet |
| CLI based | Web + GUI |

[⬆️ Back to Table of Contents](#-table-of-contents)

---

## 💻 Git Installation

Download Git from the official site:

🔗 **[Download Git](https://git-scm.com)**

### GitHub Desktop (Optional GUI)

- **Windows:** [Download for Windows](https://desktop.github.com)
- **Mac:** [Download for Mac](https://desktop.github.com)

[⬆️ Back to Table of Contents](#-table-of-contents)

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

**Verify your configuration:**

```bash
git config --list
```

[⬆️ Back to Table of Contents](#-table-of-contents)

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

**Example:**

```bash
mkdir my-project
cd my-project
git init
```

[⬆️ Back to Table of Contents](#-table-of-contents)

---

## 📂 Working Directory, Staging & Commit

Git has **3 stages**:

1. **Working Directory** – where you edit files
2. **Staging Area** – files ready for commit
3. **Repository** – committed snapshots

```
Working Directory → Staging Area → Repository
     (edit)      →  (git add)   → (git commit)
```

[⬆️ Back to Table of Contents](#-table-of-contents)

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

**Stage all files:**

```bash
git add .
```

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

**Quick commit (stage + commit):**

```bash
git commit -am "Your message"
```

[⬆️ Back to Table of Contents](#-table-of-contents)

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

**Or use (Git 2.23+):**

```bash
git switch branch_name
```

### Create and switch to new branch

```bash
git checkout -b new_branch_name
```

**Or:**

```bash
git switch -c new_branch_name
```

### Merge branch

```bash
git merge branch_name
```

### Delete branch

```bash
git branch -d branch_name
```

📌 **Branches allow parallel development.**

[⬆️ Back to Table of Contents](#-table-of-contents)

---

## 🌍 Remote Repositories

### Clone a repository

```bash
git clone repository_url
```

**Example:**

```bash
git clone https://github.com/username/repo.git
```

### Add remote

```bash
git remote add origin repository_url
```

### View remotes

```bash
git remote -v
```

### Remove remote

```bash
git remote remove origin
```

[⬆️ Back to Table of Contents](#-table-of-contents)

---

## 🔄 Sharing & Updating Code

### Fetch updates

```bash
git fetch origin
```

Fetches changes without merging.

### Pull updates

```bash
git pull
```

Fetches and merges changes.

**Pull from specific branch:**

```bash
git pull origin main
```

### Push changes

```bash
git push origin branch_name
```

**Push and set upstream:**

```bash
git push -u origin branch_name
```

[⬆️ Back to Table of Contents](#-table-of-contents)

---

## 🗂️ Tracking File Changes

### Remove file

```bash
git rm file_name
```

**Remove from Git but keep locally:**

```bash
git rm --cached file_name
```

### Rename or move file

```bash
git mv old_path new_path
```

### View movement history

```bash
git log --stat -M
```

### View file history

```bash
git log --follow file_name
```

[⬆️ Back to Table of Contents](#-table-of-contents)

---

## 📦 Temporary Commits (Stash)

### Save changes temporarily

```bash
git stash
```

**Stash with message:**

```bash
git stash save "Work in progress"
```

### View stash list

```bash
git stash list
```

### Apply stash

```bash
git stash pop
```

**Apply specific stash:**

```bash
git stash apply stash@{0}
```

### Remove stash

```bash
git stash drop
```

**Clear all stashes:**

```bash
git stash clear
```

📌 **Useful when switching branches mid-work.**

[⬆️ Back to Table of Contents](#-table-of-contents)

---

## ✍️ Rewriting History

### Rebase branch

```bash
git rebase branch_name
```

### Interactive rebase

```bash
git rebase -i HEAD~3
```

### Hard reset

```bash
git reset --hard commit_hash
```

### Soft reset

```bash
git reset --soft commit_hash
```

### Amend last commit

```bash
git commit --amend -m "New message"
```

⚠️ **Use carefully – may delete history.**

[⬆️ Back to Table of Contents](#-table-of-contents)

---

## 🔍 Inspecting & Comparing

### View commit history

```bash
git log
```

**One line view:**

```bash
git log --oneline
```

**Graph view:**

```bash
git log --graph --oneline --all
```

### Compare branches

```bash
git diff branchB...branchA
```

### Show commit details

```bash
git show commit_hash
```

### View who changed what

```bash
git blame file_name
```

[⬆️ Back to Table of Contents](#-table-of-contents)

---

## 🚫 Ignoring Files (`.gitignore`)

### Global ignore

```bash
git config --global core.excludesfile ~/.gitignore
```

### Example `.gitignore`

```gitignore
# Logs
logs/
*.log

# Dependencies
node_modules/
vendor/

# Environment files
.env
.env.local

# OS files
.DS_Store
Thumbs.db

# IDE
.vscode/
.idea/

# Build files
dist/
build/
*.notes
```

📌 **Prevents unnecessary files from being committed.**

**Useful `.gitignore` templates:** [github.com/github/gitignore](https://github.com/github/gitignore)

[⬆️ Back to Table of Contents](#-table-of-contents)

---

## ✅ Best Practices

### Commit Messages

✔️ **Good:**
```
Add user authentication feature
Fix login button alignment
Update README with installation steps
```

❌ **Bad:**
```
fix
update
changes
```

### General Best Practices

- ✔️ Write meaningful commit messages
- ✔️ Commit small, logical changes
- ✔️ Use branches for features
- ✔️ Pull before push
- ✔️ Never commit secrets or passwords
- ✔️ Use `.gitignore` properly
- ✔️ Review changes before committing
- ✔️ Keep commits atomic
- ✔️ Write descriptive branch names
- ✔️ Delete merged branches

[⬆️ Back to Table of Contents](#-table-of-contents)

---

## 🎯 Conclusion

This document provides a **complete, professional, and structured guide** to learning Git & GitHub from scratch to advanced usage.

📌 **Mastering Git is essential for:**

- 💼 Software Engineers
- 🌟 Open Source Contributors
- 👨‍💻 Professional Developers
- 🎓 Computer Science Students

### 📚 Additional Resources

- 📖 [Official Git Documentation](https://git-scm.com/doc)
- 🎓 [GitHub Learning Lab](https://lab.github.com/)
- 📺 [Git Tutorial for Beginners](https://www.youtube.com/results?search_query=git+tutorial)
- 🔗 [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)

[⬆️ Back to Table of Contents](#-table-of-contents)

---

<div align="center">

**Happy Coding! 🚀**

Made with ❤️ for developers

</div>