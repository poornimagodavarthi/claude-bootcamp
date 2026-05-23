# 🚀 Claude Code Bootcamp: Git Cheat Sheet

This guide contains the essential Git commands and workflows to stay efficient during the bootcamp.

## 💾 1. The "Save & Sync" (Basics)
Use these to save your work and update your local/remote files.

| Action | Command | What it does |
| :--- | :--- | :--- |
| **Check Status** | `git status` | Shows modified or new files. |
| **Get Latest** | `git pull origin main` | Downloads newest version from GitHub. |
| **Stage Changes** | `git add .` | Prepares ALL modified files for saving. |
| **Save Locally** | `git commit -m "msg"` | Saves staged changes with a description. |
| **Sync to Web** | `git push origin main` | Uploads local saves to GitHub. |
| **Undo Error** | `git restore <file>` | Reverts a file to its last saved state. |

---

## 🌿 2. Branching & Pull Requests (Pro Workflow)
Use branches to isolate your tasks and Pull Requests (PRs) to merge them.

| Action | Command | What it does |
| :--- | :--- | :--- |
| **New Branch** | `git checkout -b <name>` | Creates a new timeline and switches to it. |
| **Push Branch** | `git push -u origin <name>` | Uploads a new branch for the first time. |
| **Create PR** | `gh pr create` | Proposes merging your branch into `main`. |
| **View Online** | `gh browse` | Opens the current repo in your browser. |

---

## 🍴 3. The Concept of Forking
A **Fork** is your own copy of someone else's repository.
1. **Fork it**: Click the "Fork" button on the instructor's GitHub page.
2. **Clone it**: `git clone https://github.com/YOUR_USERNAME/repo-name.git`
3. **Contribute**: Push to your fork, then open a Pull Request back to the original repo.

---

## 🔄 4. The "Perfect Task Loop"
When given a new coding task:
1. `git pull origin main` (Start with the latest code).
2. `git checkout -b task-name` (Create a task branch).
3. **Let Claude write the code.**
4. `git add .` && `git commit -m "completed task-name"` (Save).
5. `git push -u origin task-name` (Upload).
6. `gh pr create --web` (Open browser to merge your work).

---

## 💡 Pro-Tips
- **Pre-Claude Save**: Before asking Claude for a massive change, run `git add .` and `git commit -m "pre-refactor"`. This gives you a perfect "Undo" point.
- **The Nuclear Undo**: If everything breaks, run `git reset --hard HEAD` to teleport back to your last save.
- **Authentication**: If it asks for a password, you are already set up to use your **Mac Login Password** or the browser-based login via `gh auth login`.
