# git_Playground
This is the remote central repository for git_Playground
# Git Command Reference

This document lists commonly used Git commands with brief explanations.


## Git Basics

git --version  [master.txt](master.txt)
→ Check installed Git version

git help  
→ Show general Git help

git help <command>  
→ Show help for a specific command
## Repository Setup

git init  
→ Initialize a new Git repository

git clone <repo_url>  
→ Clone an existing repository
## Configuration

git config --global user.name "Your Name"  
→ Set global username

git config --global user.email "you@example.com"  
→ Set global email

git config --global --list  
→ List global Git configuration

git config --local --list  
→ List repository-specific configuration
## Repository Status & History

git status  
→ Show current working tree status

git log  
→ Show commit history

git log --oneline  
→ Show compact commit history

git log --graph --oneline --all  
→ Show commit history as a graph

git show <commit>  
→ Show details of a specific commit
## Staging Files

git add <file>  
→ Stage a specific file

git add .  
→ Stage all changes in current directory

git add -A  
→ Stage all changes (including deletions)
## Committing Changes

git commit -m "message"  
→ Commit staged changes with a message

git commit -am "message"  
→ Stage tracked files and commit

## Branching

git branch  
→ List branches

git branch <branch_name>  
→ Create a new branch

git branch -d <branch_name>  
→ Delete a merged branch

git branch -D <branch_name>  
→ Force delete a branch

git switch <branch_name>  
→ Switch to a branch

git switch -c <branch_name>  
→ Create and switch to a new branch

git checkout <branch_name>  
→ Switch branches (older method)

git checkout -b <branch_name>  
→ Create and switch branch (older method)
## Merging & Rebasing

git merge <branch_name>  
→ Merge a branch into current branch

git rebase <branch_name>  
→ Reapply commits on top of another branch

git rebase --abort  
→ Cancel the rebase process
## Remote Repositories

git remote -v  
→ Show remote repositories

git remote add origin <repo_url>  
→ Add a remote repository

git remote remove origin  
→ Remove a remote repository

git remote rename origin upstream  
→ Rename a remote
## Fetching, Pulling & Pushing

git fetch  
→ Download changes without merging

git fetch origin  
→ Fetch from origin remote

git pull  
→ Fetch and merge changes

git pull origin <branch>  
→ Pull specific branch

git push  
→ Push changes to remote

git push origin <branch>  
→ Push branch to remote

git push -u origin <branch>  
→ Push and set upstream branch

git push --force  
→ Force push (overwrites history)

git push --force-with-lease  
→ Safer force push
## Undoing Changes

git restore <file>  
→ Discard changes in working directory

git restore --staged <file>  
→ Unstage a file

git checkout -- <file>  
→ Discard changes (older method)

git reset <file>  
→ Unstage file but keep changes

git reset --soft HEAD~1  
→ Undo commit, keep staged changes

git reset --mixed HEAD~1  
→ Undo commit, keep changes unstaged

git reset --hard HEAD~1  
→ Undo commit and discard changes

git revert <commit>  
→ Create a new commit that undoes another commit
## Stashing

git stash  
→ Save uncommitted changes temporarily

git stash push -m "message"  
→ Stash with description

git stash list  
→ List stashed changes

git stash show  
→ Show stash details

git stash apply  
→ Apply stash without removing it

git stash pop  
→ Apply and remove stash

git stash drop  
→ Delete a stash

git stash clear  
→ Remove all stashes
## Comparing Changes

git diff  
→ Show unstaged changes

git diff --staged  
→ Show staged changes

git diff <branch1>..<branch2>  
→ Compare two branches

git diff <commit1>..<commit2>  
→ Compare two commits

## Tags

git tag  
→ List tags

git tag <tag_name>  
→ Create lightweight tag

git tag -a <tag_name> -m "message"  
→ Create annotated tag

git push origin <tag_name>  
→ Push tag to remote

git push origin --tags  
→ Push all tags
## Ignoring Files

.gitignore  
→ Specify intentionally untracked files


