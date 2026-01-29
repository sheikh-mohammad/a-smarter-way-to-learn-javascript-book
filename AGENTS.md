# Git Workflow Instructions

## Efficient Git Workflow with Co-authorship

Follow these steps when user says `git` to add, commit with co-authorship, and push changes:

### Steps:
1. `git add <files>`
2. `git commit -m "Your commit message" -m "Co-authored-by: Qwen-Coder <qwen-coder@alibabacloud.com>"`
3. `git push origin main`

### Explanation:
- Step 1: Adds your files to the staging area
- Step 2: Creates a commit with your message and adds Qwen-Coder as a co-author
- Step 3: Pushes your changes to the remote repository

> Dont say that no commit always try to run git status.

This workflow allows you to commit changes with proper co-author attribution without creating temporary files.