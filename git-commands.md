# Git Commands Used for Lab Project

This file documents the Git commands I used throughout my lab project, following proper Git workflow and feature branching practices.

---

## 🔧 Step 1: Initialize Git

I started by initializing a Git repository in my local project folder.

```bash
git init
```

---

## 🌿 Step 2: Create Main Branch and Initial Commit

I created the `main` branch and committed my homepage files (`index.html`, styles, and assets).

```bash
git checkout -b main
git add index.html css/ assets/
git commit -m "Initial commit: Add homepage layout and styling"
```

---

## 🌱 Step 3: Create Feature Branch for Location Page

To follow proper feature branching, I created a new branch for the `location.html` file.

```bash
git checkout -b feature/location-page
```

I added and committed my work on the location page:

```bash
git add location.html css/location.css assets/location/
git commit -m "Add location page layout and related styles"
```

---

## 🔄 Step 4: Pull Latest Changes (if collaborating or working with a remote)

Before pushing my local work, I ensured my local `main` was up to date:

```bash
git checkout main
git pull origin main
```

---

## ☁️ Step 5: Push Branches to GitHub

I added the remote origin (GitHub repo):

```bash
git remote add origin https://github.com/my-username/lab-project.git
```

Then I pushed the branches:

```bash
# Push main branch
git push -u origin main

# Push feature branch
git checkout feature/location-page
git push -u origin feature/location-page
```

---

## 🛠 Step 6: Ongoing Work & Commits

As I continued working, I followed this pattern:

```bash
git add .
git commit -m "Describe what was changed"
git push origin feature/location-page
```

---

## 🔀 Optional Step: Merge Feature Branch into Main (after review)

If my feature branch is approved and ready to merge:

```bash
git checkout main
git pull origin main
git merge feature/location-page
git push origin main
```

---

## ✅ Summary of Commands Used

| Command | Purpose |
|--------|---------|
| `git init` | Start Git repository |
| `git checkout -b branch-name` | Create and switch to new branch |
| `git add` | Stage files for commit |
| `git commit -m ""` | Save changes with a message |
| `git remote add origin` | Connect to GitHub repo |
| `git push` / `git push origin branch` | Upload changes to GitHub |
| `git pull` | Sync with remote repo |
| `git merge` | Combine branches |

---
