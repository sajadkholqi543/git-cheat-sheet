# Git Cheat Sheet
🚀 The ultimate Git cheat sheet covering beginner to advanced commands, workflows, branching, rebasing, conflict resolution, and GitHub best practices.

MIT License - Free to use, share, and improve.

## Installation & Version



```bash

git --version

```



---



# Initial Configuration



### Set Username and Email



```bash

git config --global user.name "Your Name"

git config --global user.email "you@example.com"

```



### View Configuration



```bash

git config --list

```



### Edit Configuration



```bash

git config --global --edit

```



---



# Create & Clone Repositories



### Create a New Repository



```bash

git init

```



### Clone a Repository



```bash

git clone https://github.com/user/repo.git



git clone https://github.com/user/repo.git my-folder

```



---



# Check Repository Status



### Show Status



```bash

git status

```



### Short Status



```bash

git status -s

```



---



# Add Files



### Add a Single File



```bash

git add file.txt

```



### Add Multiple Files



```bash

git add file1.txt file2.txt

```



### Add Everything



```bash

git add .

```



or



```bash

git add -A

```



---



# Commit Changes



### Create a Commit



```bash

git commit -m "message"

```



### Add & Commit Tracked Files



```bash

git commit -am "message"

```



### Amend the Last Commit



```bash

git commit --amend

```



---



# View History



### Full Log



```bash

git log

```



### One-Line Log



```bash

git log --oneline

```



### Graph View



```bash

git log --graph --oneline --all

```



### Show Changes in Commits



```bash

git log -p

```



---



# Compare Changes (Diff)



### Current Changes



```bash

git diff

```



### Staged Changes



```bash

git diff --staged

```



### Compare Two Commits



```bash

git diff commit1 commit2

```



---



# Remove Files



### Remove from Git and Filesystem



```bash

git rm file.txt

```



### Remove Only from Git



```bash

git rm --cached file.txt

```



---



# Rename Files



```bash

git mv old.txt new.txt

```



---



# Branching



### List Branches



```bash

git branch

```



### Create a Branch



```bash

git branch feature

```



### Switch to a Branch



```bash

git switch feature

```



or



```bash

git checkout feature

```



### Create and Switch



```bash

git switch -c feature

```



or



```bash

git checkout -b feature

```



### Delete a Branch



```bash

git branch -d feature

```



### Force Delete



```bash

git branch -D feature

```



---



# Merge



### Merge a Branch



```bash

git merge feature

```



### Abort a Merge



```bash

git merge --abort

```



---



# Rebase



### Rebase onto Main



```bash

git rebase main

```



### Interactive Rebase



```bash

git rebase -i HEAD~5

```



### Abort Rebase



```bash

git rebase --abort

```



### Continue Rebase



```bash

git rebase --continue

```



---



# Remote Repositories



### Show Remotes



```bash

git remote -v

```



### Add a Remote



```bash

git remote add origin URL

```



### Remove a Remote



```bash

git remote remove origin

```



### Change Remote URL



```bash

git remote set-url origin URL

```



---



# Push



### First Push



```bash

git push -u origin main

```



### Regular Push



```bash

git push

```



### Force Push



```bash

git push --force

```



### Safer Force Push



```bash

git push --force-with-lease

```



---



# Pull



### Fetch and Merge



```bash

git pull

```



### Fetch and Rebase



```bash

git pull --rebase

```



---



# Fetch



### Fetch Changes



```bash

git fetch

```



### Fetch Everything



```bash

git fetch --all

```



---



# Undo Changes



### Unstage a File



```bash

git restore --staged file.txt

```



### Restore a File



```bash

git restore file.txt

```



### Reset to Previous Commit



Soft reset:



```bash

git reset --soft HEAD~1

```



Mixed reset:



```bash

git reset --mixed HEAD~1

```



Hard reset:



```bash

git reset --hard HEAD~1

```



---



# Revert



### Create an Opposite Commit



```bash

git revert COMMIT_ID

```



---



# Stash



### Save Work Temporarily



```bash

git stash

```



### List Stashes



```bash

git stash list

```



### Restore and Remove



```bash

git stash pop

```



### Restore Without Removing



```bash

git stash apply

```



### Remove One Stash



```bash

git stash drop

```



### Remove All Stashes



```bash

git stash clear

```



---



# Tags



### Create a Tag



```bash

git tag v1.0

```



### Annotated Tag



```bash

git tag -a v1.0 -m "Release"

```



### List Tags



```bash

git tag

```



### Push a Tag



```bash

git push origin v1.0

```



### Push All Tags



```bash

git push --tags

```



---



# Cherry-Pick



### Apply a Specific Commit



```bash

git cherry-pick COMMIT_ID

```



---



# Blame



### See Who Changed Each Line



```bash

git blame file.txt

```



---



# Show



### Show Commit Details



```bash

git show COMMIT_ID

```



### Show Last Commit



```bash

git show HEAD

```



---



# Clean



### Remove Untracked Files



```bash

git clean -f

```



### Remove Untracked Files & Directories



```bash

git clean -fd

```



### Dry Run



```bash

git clean -n

```



---



# Worktree



### Create a Worktree



```bash

git worktree add ../new-folder feature

```



### List Worktrees



```bash

git worktree list

```



---



# Submodules



### Add a Submodule



```bash

git submodule add URL

```



### Initialize Submodules



```bash

git submodule update --init --recursive

```



### Update Submodules



```bash

git submodule update --remote

```



---



# Bisect (Find a Bug)



Start:



```bash

git bisect start

```



Mark bad commit:



```bash

git bisect bad

```



Mark known good commit:



```bash

git bisect good COMMIT_ID

```



After testing:



```bash

git bisect good

```



or



```bash

git bisect bad

```



Finish:



```bash

git bisect reset

```



---



# Reflog (Life Saver)



### View HEAD History



```bash

git reflog

```



### Recover Lost Commit



```bash

git reset --hard HEAD@{2}

```



---



# Common GitHub Workflow



```bash

git clone URL



git switch -c feature



# make changes



git add .

git commit -m "Add feature"



git push -u origin feature



# Open Pull Request



git switch main



git pull



git merge feature



git push

```



---



# Advanced Commands



```bash

git shortlog

git describe

git archive

git fsck

git gc

git notes

git filter-branch

git replace

git rerere

git bundle

git sparse-checkout

git maintenance start

```



---



# Sample `.gitignore`



```gitignore

node_modules/

.env

dist/

build/

*.log

.vscode/

.idea/

coverage/

```



---



# 20 Essential Git Commands



```bash

git init

git clone

git status

git add .

git commit -m ""

git push

git pull

git fetch

git branch

git switch

git switch -c

git merge

git rebase

git stash

git stash pop

git log --oneline

git diff

git restore

git reset

git reflog

```



---



# Topics Every Professional Developer Should Know



* Commits

* Branches

* Merges

* Rebases

* Reset

* Revert

* Stash

* Cherry-pick

* Reflog

* Remotes / Fetch / Pull / Push

* Conflict Resolution

* Interactive Rebase

* Git Hooks

* Submodules

* Worktrees

* Git Flow

* Trunk-Based Development

Mastering these topics covers roughly **90% of what professional developers use Git for on a daily basis**.

---

## License

MIT License

Copyright (c) 2026 Sajad Kholqi

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

