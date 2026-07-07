# Git & GitHub Practice Guide

This workspace is for practicing Git and GitHub concepts step by step.

## 1. Initialize and Inspect

1. Open a terminal in `d:\demo`.
2. Run `git status` to see the current repository state.
3. Run `git log --oneline --decorate --graph --all` to view history.

## 2. Make a First Commit

1. Create or edit a file, for example `practice-file.txt`.
2. Run `git add practice-file.txt`.
3. Run `git commit -m "Add practice-file for Git exercises"`.
4. Run `git status` again.

### Real example: track notes with `notes.txt`

1. In the terminal, create a note file:
   - `echo "Hello" > notes.txt`
2. Stage the new file:
   - `git add notes.txt`
3. Commit the note:
   - `git commit -m "Add notes file"`
4. Check the commit history:
   - `git log --oneline --decorate --graph --all`

This example shows a real workflow: creating a file, staging it, and committing it as a meaningful change.

## 3. Work with Branches

1. Create a branch:
   - `git switch -c feature/notes`

   Old approach:
   - `git branch feature/notes`
   - `git switch feature/notes`
2. Edit `practice-file.txt` or create `feature-notes.txt`.
3. Commit the changes:
   - `git add .`
   - `git commit -m "Add notes on feature branch"`
4. Switch back to main:
   - `git switch main`
5. Merge the branch:
   - `git merge feature/notes`

## 4. Practice Remote GitHub Workflow

1. Create a GitHub repository on github.com.
2. Add the remote:
   - `git remote add origin https://github.com/USERNAME/REPO.git`
3. Push the main branch:
   - `git push -u origin main`
4. Create a branch, push it, and open a Pull Request.

## 5. Common Commands to Learn

- `git status`
- `git diff`
- `git add <file>`
- `git commit -m "message"`
- `git branch`
- `git switch <branch>`
- `git merge <branch>`
- `git log`
- `git remote -v`
- `git push`
- `git pull`

## 6. Additional Practice Topics

- Stashing changes: `git stash`, `git stash pop`
- Undoing commits: `git reset --soft HEAD~1`, `git revert HEAD`
- Viewing history: `git log --oneline --graph`
- Tags: `git tag v1.0`, `git push origin --tags`

## 7. Suggested Exercises

1. Create a file named `exercise-1.txt`, commit it, then modify and commit again.
2. Create a branch, add another file, then merge it into `main`.
3. Add a `.gitignore` file and commit it.
4. Push to GitHub and verify the repo history online.

---

Use this guide as your practice checklist and update it as you learn.
