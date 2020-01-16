# Git Commands

## Table of Contents

1. [Getting & Creating Projects](#project)
2. [Basic Snapshotting](#basic_commands)
3. [Branching & Merging](#branches)
4. [Working with Remote Repos](#sharing_updating)
5. [Inspection & Comparison](#inspection)
6. [Tags](#tags)
7. [Useful Links](#links)

### Getting & Creating Projects <a name="project"></a>

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone https://github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |

### Basic Snapshotting <a name="basic_commands"></a>

| Command | Description |
| ------- | ----------- |
| `git status` | Check status of working tree against HEAD |
| `git fetch` | Check for updates on remote |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add -A` | Add all new and changed files to the staging area |
| `git commit -m "[commit message]"` | Commit changes with message|
| `git commit -a -m "[commit message]"` | Add all new/changed files and commit changes with message|
| `git rm -r [file-name.txt]` | Remove a file (or folder) |
| `git rm --cached [file-name.txt]` | Remove file (or folder) from index but don't delete |

### Branching & Merging <a name="branches"></a>

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it |
| `git branch -m [old branch name] [new branch name]` | Rename a local branch |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

### Working with Remote Repos <a name="sharing_updating"></a>

| Command | Description |
| ------- | ----------- |
| `git remote -v` | View all remote branches (verbose mode) |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote rm [upstream]` | Stop tracking upstream repository |
| `git remote rename [old name] [new name]` | Rename remote repository |
| `git remote add origin https://github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin https://github.com/[[username]/[repository-name].git` | Set a repository's origin branch to HTTPS |

### Inspection & Comparison <a name="inspection"></a>

| Command | Description |
| ------- | ----------- |
| `git ls-files` | View tracked files |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git log --oneline` | View changes (briefly) |
| `git diff [source branch] [target branch]` | Preview changes before merging |

### Tags <a name="tags"></a>

| Command | Description |
| ------- | ----------- |
| `git tag` | View list of tags |
| `git tag -a [tag name] -m "[tag message]"` | Create annotated tag |
| `git show [tag name]` | View tag data |
| `git push origin [tagname]` | Push tag to remote repository |
| `git tag -d [tag name]` | Delete tag on local repo |

### Useful links <a name="links"></a>
https://www.w3docs.com/snippets/git/how-to-rename-git-local-and-remote-branches.html

https://stackoverflow.com/questions/6127328/how-can-i-delete-all-git-branches-which-have-been-merged
