# Git Fundamentals 🚀

A comprehensive quick-reference guide to fundamental Git commands, workflows, and concepts — transcribed and organized from core study notes.

---

## 📑 Table of Contents

1. [git init](#1-git-init)
2. [git clone](#2-git-clone)
3. [git status](#3-git-status)
4. [git add](#4-git-add)
5. [git commit](#5-git-commit)
6. [git push](#6-git-push)
7. [git pull](#7-git-pull)
8. [git fetch](#8-git-fetch)
9. [git checkout & git switch](#9-git-checkout--git-switch)
10. [git merge](#10-git-merge)
11. [git rebase](#11-git-rebase)
12. [git log](#12-git-log)
13. [git diff](#13-git-diff)
14. [git stash](#14-git-stash)
15. [git reset](#15-git-reset)
16. [git revert](#16-git-revert)
17. [git cherry-pick](#17-git-cherry-pick)
18. [git tag](#18-git-tag)

---

## 1. `git init`

A Git command used to initialize a new Git repository in a project folder. It allows Git to track changes in your files.

### Example
```bash
# 1. Create a project folder
mkdir myproject

# 2. Open the project folder
cd myproject

# 3. Initialize git in that folder
git init
```

**Output:**
```text
Initialized empty Git repository in /path/to/myproject/.git/
```

> **Remember:** Start tracking a project with Git.

---

## 2. `git clone`

A Git command used to copy an existing Git repository from GitHub (or any remote host) to your local machine.

### Example
```bash
git clone https://github.com/username/repository.git
```

> **Remember:** Copy an existing repository to your computer.

---

## 3. `git status`

A Git command used to check the current state of your working directory and staging area.

### Example
```bash
git status
```

> **Remember:** Check the current state of your Git repository.

---

## 4. `git add`

A Git command used to add new or modified files to the staging area before committing them.

### Example
```bash
git add index.html

# Or stage all modified and new files:
git add .
```

> **Remember:** Prepare files for commit.

---

## 5. `git commit`

A Git command used to save staged changes to the repository with a descriptive message.

### Example
```bash
git commit -m "Added Homepage"
```

### Explanation
- `git commit`: Saves the staged changes in the repository history.
- `-m`: Adds a message describing the changes.
- `"Added Homepage"`: Describes what you changed.

> **Remember:** Save staged changes with a descriptive message.

---

## 6. `git push`

A Git command used to upload your local commits to a remote repository, such as GitHub.

### Example
```bash
git push origin main
```

### Explanation
- `git push`: Uploads your committed changes.
- `origin`: The default name given to the remote repository.
- `main`: The branch where you want to upload your changes.

> **Remember:** Upload your committed code to GitHub.

---

## 7. `git pull`

A Git command used to download the latest changes from a remote repository (such as GitHub) and integrate them directly into your current local branch.

### Example
```bash
git pull origin main
```

### Explanation
- `git pull`: Fetches and integrates remote changes into your working branch.
- `origin`: The name of the remote repository.
- `main`: The branch from which you want to retrieve changes.

> **Remember:** Get the latest changes from GitHub & integrate them into your local project.

---

## 8. `git fetch`

A Git command used to download the latest updates from a remote repository without automatically merging them into your current branch.

### Example
```bash
git fetch origin
```

### Explanation
- `git fetch`: Downloads metadata and commits from the remote repository.
- `origin`: The name of the remote repository.

### Comparison: `git fetch` vs `git pull`

| Command | Downloads Updates? | Merges into Current Branch? |
|---|:---:|:---:|
| `git fetch` | ✅ Yes | ❌ No (safe inspection) |
| `git pull` | ✅ Yes | ✅ Yes (`fetch` + `merge`) |

---

## 9. `git checkout` & `git switch`

A Git command used to switch branches or restore working tree files.

### Example
```bash
# Switch to an existing branch
git checkout feature
```

> **Note:** `git switch` is the modern, clearer command specifically designed for switching branches, though `git checkout` remains widely used.

```bash
# Modern syntax to switch branches:
git switch feature

# Create and switch to a new branch:
git switch -c feature-name
```

> **Remember:** Switch branches or restore files.

---

## 10. `git merge`

A Git command used to combine changes from one branch into another branch.

### Example
```bash
git switch main
git merge feature
```

### Explanation
- `git switch main`: Switches to the target branch (`main`).
- `git merge feature`: Combines changes from the `feature` branch into `main`.

> **Remember:** Combine changes from one branch into another.

---

## 11. `git rebase`

A Git command used to move or replay commits from one branch onto another branch, creating a cleaner, more linear project history.

### Example
```bash
git switch feature
git rebase main
```

### Explanation
- `git switch feature`: Switches to your feature branch.
- `git rebase main`: Replays your feature branch's commits on top of the latest `main` branch.

### Comparison: `git merge` vs `git rebase`

| Feature | `git merge` | `git rebase` |
|---|---|---|
| **History Structure** | Combines branch histories, branching graph | Replays commits onto another base, linear history |
| **Merge Commits** | May create a separate merge commit | Does not create a merge commit |
| **Commit Hashes** | Preserves existing commit IDs | Creates new commit IDs for replayed commits |

> **Remember:** Replay your commits on top of another branch to create a cleaner history.

---

## 12. `git log`

A Git command used to view the commit history of a repository, including commit IDs (SHA-1 hashes), authors, dates, and commit messages.

### Example
```bash
git log
```

**Sample Output:**
```text
commit a1b2c3d4e5f6...
Author: Kuvalesh <user@example.com>
Date:   Mon Oct 19 10:00:00 2026

    Initial commit.
```

> **Remember:** View the history of commits in Git.

---

## 13. `git diff`

A Git command used to compare changes between files, commits, or branches.

### Example
```bash
git diff
```

**Sample Output:**
```diff
- Hello world
+ Hello git
```
- `-` indicates a line was removed.
- `+` indicates a line was added.

> **Remember:** Compare changes in your code.

---

## 14. `git stash`

A Git command used to temporarily save (stash) your uncommitted changes so you can work on something else without committing incomplete work.

### Useful Commands
```bash
# Save modified working directory changes temporarily
git stash

# View list of saved stashes
git stash list

# Restore the most recent stash and remove it from the stash list
git stash pop

# Restore the stash changes while keeping it saved in the stash list
git stash apply
```

> **Remember:** Temporarily save your uncommitted changes.

---

## 15. `git reset`

A Git command used to move the current branch HEAD to a previous commit or remove files from the staging area.

### Example
```bash
git reset index.html
```
- Removes `index.html` from the staging area while preserving your working file changes.

> **Remember:** Move the branch back or undo staging.

---

## 16. `git revert`

A Git command used to undo the changes introduced by a previous commit by creating a brand-new commit.

### Example
```bash
git revert HEAD
```

### Explanation
- `git revert`: Safely reverses changes by appending an inverse commit.
- `HEAD`: Points to the current/latest commit.

### Comparison: `git reset` vs `git revert`

| Feature | `git reset` | `git revert` |
|---|---|---|
| **Action** | Moves the branch pointer backward | Creates a new commit to undo changes |
| **History** | Can rewrite/truncate commit history | Preserves complete history |
| **Collaboration** | Use carefully on shared/public branches | Generally safe for shared/public branches |

> **Remember:** Undo a commit safely without deleting history.

---

## 17. `git cherry-pick`

A Git command used to apply the changes from a specific commit from one branch into another branch without merging the entire branch.

### Example
```bash
git switch main
git cherry-pick a1b2c3d
```

### Explanation
- `git switch main`: Switches to your target branch.
- `git cherry-pick a1b2c3d`: Copies and applies the changes from commit `a1b2c3d`.

> **Remember:** Select and apply a specific commit from another branch.

---

## 18. `git tag`

A Git command used to mark and label a specific commit in history (commonly used for version releases like `v1.0.0`).

### Useful Commands
```bash
# List all tags in the repository
git tag

# Create a lightweight tag
git tag v1.0

# View tag details and the associated commit
git show v1.0

# Push a specific tag to the remote repository (GitHub)
git push origin v1.0

# Push all local tags to the remote repository
git push origin --tags
```

> **Remember:** Mark a specific release version of your project.
