# A02 — Tutorial on Using **GIT** and **Github** with WebStorm

This tutorial explains how to use **GIT**, **Github**, and WebStorm to create and manage a **Repository**. It is written so that another student can follow the steps to complete the assignment.  

---

## Part 1: Step-by-Step Directions Using WebStorm

### Step 1: Install Required Software
- **Github** account: https://github.com/join  
- **GIT**: https://git-scm.com/downloads  
- **Git for Windows** (if on Windows): https://gitforwindows.org  
- **WebStorm IDE**: https://www.jetbrains.com/webstorm/download/  

---

### Step 2: Create a Remote **Repository** on **Github**
1. Log in to **Github**.  
2. In the top-right corner, click the **+** sign → **New repository**.  
3. Name the repository exactly: `A02` (capital **A**).  
4. Select Public or Private as required.  
5. Optionally check **Add a README file**.  
6. Click **Create repository**.  

---

### Step 3: **Clone** the **Repository** Locally
You must make a local copy of the **Repository** on your computer.  

- Copy the HTTPS URL (looks like `https://github.com/yourUCID/A02.git`).  

From terminal:
```bash
git clone https://github.com/yourUCID/A02.git
cd A02

git config --global user.name "Your Name"
git config --global user.email "you@school.edu"
git --version   # check if installed
```
From WebStorm:

On the welcome screen → Get from VCS.

Paste the repo URL.

Click Clone.

### Step 4: Configure GIT (first time only)

Run these commands in the terminal:

```
git config --global user.name "Your Name"
git config --global user.email "you@school.edu"
git --version   # check if installed
 ```
### Step 5: Editing Files in WebStorm
Open the A02 project folder in WebStorm (File → Open).
Add or edit files (e.g., edit README.md).
Save changes.

###Step 6: Commit and Push Changes
When you make progress:
In WebStorm, open the Commit window (VCS → Commit).
Write a clear Commit message, such as:
Task: Create Repository
Feature: added workflow for using github
Fix: changed readme.md for definition of terms
Click Commit and Push.

This will send your work from local files to the Remote Repository on Github.

### Step 7: Working with Branches

In WebStorm → Git widget (bottom right) → New Branch.

Name it (e.g., feature/readme).

Work in this branch and Commit changes.

Switch back to main → Merge the branch.

### Step 8: Handling a Merge Conflict
If two branches change the same lines of code, you may see a Merge Conflict.

WebStorm highlights conflicts.

Use the merge tool to pick or combine changes.

Mark conflicts resolved and Commit.

### Step 9: Syncing with Remote

git fetch → download changes from Remote without merging.

git pull → fetch + merge (updates your local branch).

git push → upload local commits to Github.

### Step 10: Submitting the Repository
Verify the repo URL looks like:
```
https://github.com/yourUCID/A02

```
Paste this URL into Canvas and submit.

### Glossary of Terms

**Branch** — A separate line of development in a Repository.

**Clone** — Making a local copy of a Repository from Github.

**Commit** — Saving a snapshot of your changes in GIT.

**Fetch** — Downloading updates from the Remote without merging them into your local branch.

**GIT** — A distributed version control system for tracking changes.

**Github** — A cloud hosting service for GIT repositories.

**Merge** — Combining one Branch into another.

**Merge Conflict** — When GIT cannot automatically reconcile differences between Branches.

**Push** — Uploading local commits to a Remote Repository.

**Pull** — Fetching and merging updates from a Remote Repository.

**Remote** — The version of your Repository stored on a server like Github.

**Repository** — A project folder tracked by GIT that contains files, history, and Branches.

### References

Git official documentation: https://git-scm.com
GitHub Docs — Repositories: https://docs.github.com/en/repositories
Git for Windows: https://gitforwindows.org
WebStorm download: https://www.jetbrains.com/webstorm/download/
Git Cheat Sheet: https://education.github.com/git-cheat-sheet-education.pdf
