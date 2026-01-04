# 🚀 Git & GitHub Complete Learning Guide  
*A Professional & Beginner-Friendly Documentation*

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

This document is a **complete Git & GitHub learning guide** created from the official **GitHub Education Git Cheat Sheet** and expanded with **clear explanations**, **real-world usage**, and **professional standards**.

It is suitable for:
- Beginners 🚀
- Students 🎓
- Junior Developers 💻
- Professional Teams 🏢

---

## 🔧 What is Git?

**Git** is a **free and open-source distributed version control system**.

### 🔹 Why Git?
- Tracks code changes
- Maintains history
- Enables team collaboration
- Prevents code loss
- Allows rollback to previous versions

📌 Git works **locally on your computer**.

---

## 🌐 What is GitHub?

**GitHub** is a **cloud-based platform** that hosts Git repositories.

### 🔹 Why GitHub?
- Store code online
- Collaborate with teams
- Share projects
- Manage issues & pull requests
- CI/CD & automation

📌 GitHub uses **Git internally**.

---

## ⚖️ Git vs GitHub

| Git | GitHub |
|----|-------|
| Local tool | Online platform |
| Version control | Code hosting |
| Works offline | Requires internet |
| CLI based | Web + GUI |

---

## 💻 Git Installation

Download Git from the official site:

🔗 https://git-scm.com

### GitHub Desktop (Optional GUI)
- Windows: https://windows.github.com  
- Mac: https://mac.github.com  

---

## ⚙️ Initial Git Setup

Configure your identity (required):

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"

Enable colored output:

git config --global color.ui auto

📁 Git Repository & git init
🔹 What is a Repository?

A Git repository is a folder where Git tracks all changes.

🔹 git init Definition
git init


Initializes a directory as a Git repository
It creates a hidden .git folder that stores:

Commit history

Branches

Configuration

📌 Use this when starting a new project.

📂 Working Directory, Staging & Commit
Git has 3 stages:

Working Directory – where you edit files

Staging Area – files ready for commit

Repository – committed snapshots

🧩 Basic Git Commands
Check status
git status


Shows modified, staged, and untracked files.

Stage a file
git add file_name


Adds file to the staging area.

Unstage a file
git reset file_name


Removes file from staging but keeps changes.

View changes
git diff


Shows unstaged changes.

git diff --staged


Shows staged changes.

Commit changes
git commit -m "Descriptive commit message"


Creates a snapshot of staged files.

🌿 Branching & Merging
List branches
git branch

Create a new branch
git branch branch_name

Switch branch
git checkout branch_name

Merge branch
git merge branch_name


📌 Branches allow parallel development.

🌍 Remote Repositories
Clone a repository
git clone repository_url

Add remote
git remote add origin repository_url

🔄 Sharing & Updating Code
Fetch updates
git fetch origin

Pull updates
git pull

Push changes
git push origin branch_name

🗂️ Tracking File Changes
Remove file
git rm file_name

Rename or move file
git mv old_path new_path

View movement history
git log --stat -M

📦 Temporary Commits (Stash)
Save changes temporarily
git stash

View stash list
git stash list

Apply stash
git stash pop

Remove stash
git stash drop


📌 Useful when switching branches mid-work.

✍️ Rewriting History
Rebase branch
git rebase branch_name

Hard reset
git reset --hard commit_hash


⚠️ Use carefully – may delete history.

🔍 Inspecting & Comparing
View commit history
git log

Compare branches
git diff branchB...branchA

Show commit details
git show commit_hash

🚫 Ignoring Files (.gitignore)
Global ignore
git config --global core.excludesfile ~/.gitignore

Example .gitignore
logs/
*.notes
node_modules/
.env


📌 Prevents unnecessary files from being committed.

✅ Best Practices

✔ Write meaningful commit messages
✔ Commit small changes
✔ Use branches
✔ Pull before push
✔ Never commit secrets
✔ Use .gitignore

🎯 Conclusion

This document provides a complete, professional, and structured guide to learning Git & GitHub from scratch to advanced usage.

📌 Mastering Git is essential for:

Software Engineers

Open Source Contributors

Professional Developers