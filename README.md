# GitHub Practice

A small repository for practicing Git and GitHub workflows.

## What I practiced

- Practiced restoring changes with Git.
- Worked with feature branches, including `feature-profile`, `feature-login`, `feature-payment`, and `feature-conflict`.
- Made changes on `main` and a feature branch that conflicted in `conflict.txt`.
- Resolved the merge conflict and committed the resolved file.

## Commands practiced

### Check the working tree

```bash
git status
git log --oneline --decorate
git branch
```

### Create and switch branches

```bash
git switch -c feature-profile
git switch main
```

Create a branch from the current branch with `git switch -c`, and use `git switch` to move between existing branches.

### Stage, commit, and restore changes

```bash
git add profile.txt
git commit -m "Add profile feature"
```

Discard unstaged changes to a tracked file, or unstage a file while keeping its changes:

```bash
git restore profile.txt
git restore --staged profile.txt
```

Use `git restore <file>` to discard unstaged changes to a tracked file. Use `git restore --staged <file>` to unstage a file while keeping its working-tree changes.

### Merge a feature branch

```bash
git switch main
git merge feature-conflict
```

If Git reports a conflict, edit the conflicted file (such as `conflict.txt`) to keep the desired content and remove the conflict markers. Then stage and commit the resolution:

```bash
git add conflict.txt
git commit -m "Resolve merge conflict"
```

### Push commits to GitHub

```bash
git push origin main
```

## Practice files

- `day2.txt` — notes from Git Day 2 practice.
- `profile.txt` — profile feature practice.
- `conflict.txt` — example of a resolved merge conflict.



https://chatgpt.com/c/6adc7cd4-8c40-83ee-8c8c-25460da567d2