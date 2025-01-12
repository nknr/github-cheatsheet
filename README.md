
## Initialization

| Command                                  | Description                                               |
|:-----------------------------------------|:----------------------------------------------------------|
| `git init`                               | Initialize Git into the local directory                   |
| `git remote add origin [repository url]` | Specifies the remote repository for your local repository | 
| `git clone [repository url]`             | Clone(download) remote repository into local directory    |
| `git push -u <remote> <branch>`          | It pushes the current branch’s commits to the specified remote branch. | 

#### What git push -u Does
- Pushes Changes:
     1. It pushes the current branch’s commits to the specified remote branch.
- Sets Upstream:
     1. The <b>-u or --set-upstream</b> flag sets the remote branch as the upstream for your local branch.
     2.	This allows you to use simple commands like git push and git pull in the future without specifying the remote and branch.

## Branch

| Command                                   | Description                                          |
|:------------------------------------------|:-----------------------------------------------------|
| `git branch`                              | Display working branch name                          |
| `git branch [branch-name]`                | Create a new branch                                  |
| `git switch [branch-name]`                | Switches to the specified branch                     |
| `git checkout [branch-name]`              | Switches to the specified branch                     |
| `git checkout -b [branch-name]`           | Create new branch & switches to the specified branch |
| `git checkout [branch-name] -- file name` | Checkout to a specified file                         |
| `git checkout [Commint-Id]`               | Create new branch & switches to the specified branch |
| `git branch -d [branch-name]`             | Delete specified branch from local directory         |

**Switch vs Checkout** `switch` is a new command introduced in Git 2.23 (released in August 2019).
Its primary purpose is to simplify the process of switching between branches while in `checkout` is a versatile Git command that can be used for a variety of purposes, including switching branches, creating new branches, and even checking out specific files or commits

### Changes

| Command                                     | Description                                                                                |
|:--------------------------------------------|:-------------------------------------------------------------------------------------------|
| `git add .`                                 | Add all changes to stage area                                                              |
| `git add [file]`                            | Add specified file to stage area                                                           |
| `git commit -m "[message]"`                 | Commit staged file in version history                                                      |
| `git commit -a`                             | Commit staged file in version history                                                      |
| `git status`                                | Show all file which are modified, created, deleted, un-staged file                         |
| `git diff`                                  | Show all changes which are not staged                                                      |
| `git diff -staged`                          | Shows the differences between the files in the staging area and the latest version present |
| `git rm [file]`                             | Delete un-staged file                                                                      |
| `git rm -f [file]`                          | Delete file                                                                                |
| `git merge [branch name]`                   | Merge a branch into the active branch                                                      |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch                                                        |
| `git stash`                                 | Stash changes in a dirty working directory                                                 |
| `git stash clear`                           | Remove all stashed entries                                                                 |
| `git stash save "message"`                  | Save changes in a dirty working directory with message                                     |
| `git stash list`                            | Show all saved change list                                                                 |
| `git stash apply [index]`                   | Copy save change to directory                                                              |
| `git stash drop [index]`                    | Copy save the change to the directory and clear changes from stash                         |
| `git push`                                  | Sends committed changes in repository                                                      |


**Untracked files** are files that have been created within your repo's working directory but have not yet been added to the repository's tracking index using the `git add` command
