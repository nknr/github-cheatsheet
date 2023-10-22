
### Initialization

| Command                                  | Description                                               |
|:-----------------------------------------|:----------------------------------------------------------|
| `git init`                               | Initialize Git into the local directory                   |
| `git remote add origin [repository url]` | Specifies the remote repository for your local repository | 
| `git clone [repository url]`             | Clone(download) remote repository into local directory    |

### Branch

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

| Command                     | Description                           |
|:----------------------------|:--------------------------------------|
| `git add .`                 | Add all changes to stage area         |
| `git add [file]`            | Add specified file to stage area      |
| `git commit -m "[message]"` | Commit staged file in version history |
| `git commit -a"`            | Commit staged file in version history |


