#  Git Essentials Cheat Sheet

A quick reference guide to the most common Git commands for beginners and developers.

---

##  `git init` — Initialize a Git Repository

**Purpose:**  
Initializes a new Git repository in your current directory.

**What It Does:**
- Creates a hidden `.git/` directory.
- Starts version control on the project.

**Usage:**
```bash
mkdir my-project
cd my-project
git init
```

## git status — Show Current State
Purpose:
Displays the status of your working directory and staging area.

## What It Shows:

- Modified but unstaged files

- Staged files ready to commit

- Untracked files

- Current branch info

```bash
git status
```
```bash
On branch main
Changes not staged for commit:
  modified:   style.css

Untracked files:
  newfile.js

```
## git add . — Stage All Changes
### Purpose:
- Stages all modified and untracked files.
- Includes all files in the current and subdirectories (except .gitignored files).

```bash
git add .
```

git commit -m "message" — Save Staged Changes
Purpose:
Commits staged changes with a descriptive message.
Saves a snapshot of your project to local history.
```bash
git commit -m "Added homepage layout and CSS styles"
```

## git log — View Commit History
### Purpose:
Displays a list of previous commits.

Usage:
```bash
git log
```
Output:

```bash
commit 1a2b3c4d5e...
Author: Jane Doe <jane@example.com>
Date:   Tue Apr 30 14:12:45 2025 +0530
```

## git checkout <commit-hash> — Switch to a Specific Commit
### Purpose:
- Restores your project to a previous commit state using its hash.
- You’ll enter a detached HEAD state — not on any branch.

Usage:
```bash
git checkout 1a2b3c4d
```
Create a new branch from that state:
```bash
git checkout -b new-feature-branch 1a2b3c4d
```
