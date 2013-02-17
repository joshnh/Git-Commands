Git Commands
============

A list of commonly used Git commands:

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository | 
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add -A` | Add all new and changed files to the staging area |
| `git commit -m "[commit message]"` | Commit changes |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git remote add origin ssh://git@github.com/joshnh/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/joshnh/[repository-name].git` | Set a repository's origin branch to SSH |
| `git push -u origin [branch name]` | Push changes to remote repository (first time) |
| `git push` | Push changes to remote repository (subsequent times) |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git clone ssh://git@github.com/joshnh/[repository-name].git` | Create a local copy of a remote repository |
| `git branch [branch name]` | Create a new branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [branch name] [target branch]` | Merge a branch into a target branch |
| `git diff [source branch] [target branch}` | Preview changes before merging |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |
