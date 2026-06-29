# 📚 GitHub Flow - Cheat Sheet

## What is GitHub Flow?

GitHub Flow is a simple workflow used to develop features, fix bugs, and collaborate safely without modifying the `main` branch directly.

---

# Typical Workflow

```text
1. Clone the repository
2. Create a new branch
3. Make changes
4. Commit changes
5. Push the branch
6. Open a Pull Request
7. Review and merge
8. Delete the branch
```

---

# Clone a Repository

```bash
git clone <repository_url>
cd repository_name
```

---

# Check Repository Status

```bash
git status
```

---

# Create a New Branch

```bash
git checkout -b feature_branch
```

Example:

```bash
git checkout -b feature/readme-update
```

---

# Verify Current Branch

```bash
git branch
```

The current branch is marked with `*`.

---

# Make Changes

Edit your files, then check the changes:

```bash
git status
```

---

# Stage Changes

One file:

```bash
git add filename
```

All files:

```bash
git add .
```

---

# Commit Changes

```bash
git commit -m "Add README improvements"
```

---

# Push the Branch

First push:

```bash
git push -u origin feature/readme-update
```

Next pushes:

```bash
git push
```

---

# Keep Your Branch Updated

```bash
git fetch origin
git rebase origin/main
```

---

# Switch Branches

```bash
git checkout main
```

```bash
git checkout feature/readme-update
```

---

# Merge Changes

After the Pull Request is approved:

```bash
git checkout main
git pull
git merge feature/readme-update
```

---

# Delete a Branch

Local branch:

```bash
git branch -d feature/readme-update
```

Remote branch:

```bash
git push origin --delete feature/readme-update
```

---

# Useful Commands

View commit history:

```bash
git log --oneline
```

Display remote repositories:

```bash
git remote -v
```

Restore a file:

```bash
git restore filename
```

---

# Good Practices

* Never work directly on `main`.
* Create one branch for one feature or one bug fix.
* Write meaningful commit messages.
* Pull or fetch regularly.
* Check `git status` before committing.
* Test your work before creating a Pull Request.

---

# What I Learned

* Create and manage branches.
* Work independently without affecting `main`.
* Commit changes with meaningful messages.
* Push branches to GitHub.
* Keep branches synchronized.
* Merge completed work safely.
* Follow the GitHub Flow workflow.

