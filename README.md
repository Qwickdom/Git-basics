<div align="center">

 # Introduction to Git
 
 <p> A version control system like Git helps us to keep the history of changes and growth of our project files. <br>
  In reality, changes and differences between versions of our projects can have similarities, sometimes the changes can be just a word or a specific part of a specific file. Git is optimized to save all these changes atomically and incrementally, that is, applying changes on the last changes, these on the previous changes and so on until the beginning of our project. </p>

 ## Basic Commands

 | Commands                    | Description                                                   |
 | --------------------------- | ------------------------------------------------------------- |
 | `git add [file.txt]`        | Add a file to the _Staging_ area                              |
 | `git add -A`                | Add all new and changed files to the staging area             |
 | `git clone https://github.com/[user]/[repository].git` | Create a local copy of a remote repository |
 | `git commit -m "message"`   | Commit changes                                                |
 | `git config --global user.email your@email.com`        | Configure an email                 |
 | `git config --global user.name [Name]`                 | Configure a name                   |
 | `git config --list`         | List the configurations                                       |
 | `git init`                  | Initialize a local Git repository                             |
 | `git log`                   | View changes history                                          |
 | `git pull`                  | Update local repository to the newest commit                  |
 | `git push`                  | Push changes to remote repository (remembered branch)         |
 | `git rm -r [file-name.txt]` | Remove a file (or folder)                                     |
 | `git rm --cached [file/s]`  | Removes the files from the _Staging_ area and the next commit |
 | `git rm --force [file/s]`   | Delete files in Git and locally. We can recover them          |
 | `git show`                  | Show latest changes                                           |
 | `git status`                | Check status                                                  |

 ## Inspection & Comparison

 | Commands            | Description                                |
 | ------------------- | ------------------------------------------ |
 | `git diff [source branch] [target branch]`   | Preview changes before merging                     |
 | `git log`           | View changes                               |
 | `git log --all --graph --decorate --oneline` | Shows the history of the repository in a graphical |
 | `git log --oneline` | View changes (briefly)                     |
 | `git log --stat`    | Shows the number of bytes added or deleted |
 | `git log --summary` | View changes (detailed)                    |

 ## Branching & Merging

 | Command                                     | Description                                             |
 | ------------------------------------------- | ------------------------------------------------------- |
 | `git branch`                                | List branches (the asterisk denotes the current branch) |
 | `git branch [branch name]`                  | Create a new branch                                     |
 | `git branch -a`                             | List all branches (local and remote)                    |
 | `git branch -d [branch name]`               | Delete a branch                                         |
 | `git branch -m [old branch name] [new branch name]` | Rename a local branch                           |
 | `git merge [branch name]`                   | Merge a branch into the active branch                   |
 | `git merge [source branch] [target branch]` | Merge a branch into a target branch                     |
 | `git push origin --delete [branch name]`    | Delete a remote branch                                  |
 | `git stash`                                 | Stash changes in a dirty working directory              |
 | `git stash clear`                           | Remove all stashed entries                              |

 ## Back in time with branches and checkout
 
 | Commands                                  | Description                                            |
 | ----------------------------------------- | ------------------------------------------------------ |
 | `git checkout [commit/branch] [filename]` | Allows you to return to the specified commit or branch |
 | `git checkout -`                          | Switch to the branch last checked out                  |
 | `git checkout -– [file-name.txt]`         | Undo changes to a file in a modified state             |
 | `git checkout -b [branch name]`           | Create a new branch and switch to it                   |
 | `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it      |
 | `git reset HEAD`                          | It only removes them from the staging area             |
 | `git reset [commit] --soft/hard`          | Returns to the specified commit; removing all changes  |
</div>
