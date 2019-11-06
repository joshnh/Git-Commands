Git Commands
============

## Translated Versions
- [Versão em português](READMEpt.md)

___

_A list of my commonly used Git commands_

*If you are interested in my Git aliases, have a look at my `.bash_profile`, found here: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |
| `git clone ssh://git@github.com/[username]/[repository-name]. git  foldername` | Create a local copy of a remote repository and save them in new created foldername folder |

### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add --A` | Add all new and changed files to the staging area #method-1|
| `git add .` | Add all new and changed files to the staging area #method-2|
| `git commit -m "[commit message]"` | Commit changes |
| `git commit –amend` | Merge new commit to previous commit |
| `git commit -a -m "[commit message]"` | Staged track file and didn’t changed, add or commit untracked file |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |
| `git rm "[filename.txt]"` | Remove file and staged change |
| `rm -rf "[file-name.txt]"` | Remove a file (or folder) |
| `git rm –cached "[filename]"` | Already tracking file remove from track and staged them |
| `git mv [initial-file-Name] [rename-file-name]` |Changed name of file from initialfileName to renamefile and staged them |

### Branching & Merging

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

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git log --oneline` | View changes (briefly) |
| `git log -p` | Display commit with what you changed in file also display |
| `git log -p -3` |  Display last 3 commit with what you changed in file / along diff |
| `git log –stat` | Show commit with shortest summary |
| `git log –pretty=oneline` | Show all commit in line by line |
| `git log –pretty=short` | Show only commit message ,author|
| `git log –pretty=full` | Show commit message , author and committed person detail |
| `git log –since=2.days/weeks/months/years` | Show commit of last 2 days, week,months or year |
| `git diff [source branch] [target branch]` | Preview changes before merging |
| `git diff` | Display difference of working directory with staging area|
| `git diff –staged` | Compare previous commit with new staging area |
