---
layout: "page-w-col"
title: "Git"
subtitle: "Workshops, how-to-use, commands, and more!"
links:
  - link: "https://git-scm.com/"
    title: "Git Website"
  - link: "https://github.com"
    title: "Github"
  - link: "https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet"
    title: "Github Markdown Cheatsheet"
---
### Next workshop: Thursday, October 15th

We are planning to use BR 164 for the workshop but this is subject to change.


### What is Git?
_Git_ is a distributed version control system.
It is one skill every software professional is
bound to find necessary in their career. We use it here
to run our website and do other cool stuff. You
will learn how to manage your projects better with
Git and be introduced to the popular code sharing
website github.com. Participants also get a tiny
surprise gift.



### Git Commands
Source: [siteground.com](https://www.siteground.com/tutorials/git/commands.htm)

| Command | Description |
|:--------|:-------:|
| git config - -global user.name "My Name"  | Sets the users name for the git installation.  This is required to use with GitHub   |
| git config - -global user.email "name@domain.com"  | Sets the users email for the git installation.  This is required to use with GitHub   |
|  git init   | Initializes a git repository – creates the initial ‘.git’ directory in a new or in an existing project.  |
| git clone   | Makes a Git repository copy from a remote source. Also adds the original location as a remote so you can fetch from it again and push to it if you have permissions. Example: git clone git@github.com:user/test.git   |
| git add | Adds files changes in your working directory to your index. Example: git add .   |
| git rm | Removes files from your index and your working directory so they will not be tracked. Example: git rm filename |
| git commit | Takes all of the changes written in the index, creates a new commit object pointing to it and sets the branch to point to that new commit. Examples: git commit -m ‘committing added changes’ git commit -a -m ‘committing all changes, equals to git add and git commit’   |
| git status | Shows you the status of files in the index versus the working directory. It will list out files that are untracked (only in your working directory), modified (tracked but not yet updated in your index), and staged (added to your index and ready for committing). Example: git status # On branch master # # Initial commit # # Untracked files: # (use "git add <file>..." to include in what will be committed) # # README nothing added to commit but untracked files present (use "git add" to track)   |
| git branch | Lists existing branches, including remote branches if ‘-a’ is provided. Creates a new branch if a branch name is provided. Example: git branch -a * master remotes/origin/master   |
| git checkout | Checks out a different branch – switches branches by updating the index, working tree, and HEAD to reflect the chosen branch. Example: git checkout newbranch  |
| git merge | Merges one or more branches into your current branch and automatically creates a new commit if there are no conflicts. Example: git merge newbranchversion  |
| git reset | Resets your index and working directory to the state of your last commit. Example: git reset --hard HEAD  |
| git stash | Temporarily saves changes that you don’t want to commit immediately. You can apply the changes later. Example: git stash Saved working directory and index state "WIP on master: 84f241e first commit" HEAD is now at 84f241e first commit (To restore them type "git stash apply")   |
| git tag | Tags a specific commit with a simple, human readable handle that never moves. Example: git tag -a v1.0 -m 'this is version 1.0 tag'  |
| git fetch | Fetches all the objects from the remote repository that are not present in the local one. Example: git fetch origin  |
| git pull | Fetches the files from the remote repository and merges it with your local one. This command is equal to the git fetch and the git merge sequence. Example: git pull origin  |
| git push | Pushes all the modified local objects to the remote repository and advances its branches. Example: git push origin master   |
| git remote | Shows all the remote versions of your repository. Example: git remote origin  |
| git log | Shows a listing of commits on a branch including the corresponding details. Example: git log commit 84f241e8a0d768fb37ff7ad40e294b61a99a0abe Author: User <user@domain.com> Date: Mon May 3 09:24:05 2010 +0300 first commit   |
|=====
| git diff | Generates patch files or statistics of differences between paths or files in your git repository, or your index or your working directory. Example: git diff
{: class="table"}
