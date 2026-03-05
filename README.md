# Git Reference Practice

Basic Git usage demonstration project.

## Video Tutorial

Watch the full tutorial: [Git Basics Demo](https://www.youtube.com/watch?v=2FVuRnv7g-0&t=82s)

## Git Workflow

```
Working Directory  →  Staging Area  →  Local Repository  →  Remote Repository
     (edit)           (git add)        (git commit)         (git push)
                          ↓                  ↓                    ↓
                       [Index]          [.git folder]         [GitHub]
```

## Branching Flow

```
main    ──●──────●──────●──────●────
           \              /
  feature   ●────●────●──
           (branch)  (merge)
```

## Commands Covered

```bash
# Initialize repository
git init

# Stage changes
git add <file>
git add .

# Commit changes
git commit -m "message"

# Check status
git status

# View history
git log

# Create branch
git branch <branch-name>

# Switch branch
git checkout <branch-name>

# Merge branch
git merge <branch-name>

# Remote operations
git remote add origin <url>
git push origin <branch>
git pull origin <branch>
```

## Common Scenarios

```bash
# Start new project
git init
git add .
git commit -m "Initial commit"

# Clone existing project
git clone <repo-url>

# Create feature branch
git checkout -b feature-name
# ... make changes ...
git add .
git commit -m "Add feature"
git checkout main
git merge feature-name

# Undo changes
git restore <file>          # Discard working changes
git reset HEAD <file>       # Unstage file
git revert <commit-hash>    # Undo commit
```
