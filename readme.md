# Git Cheatsheet 🎮

Welcome to the Git Cheat Sheet! This comprehensive guide contains essential Git commands for developers of all skill levels. Whether you're just starting out or you're an experienced programmer, this cheat sheet is a handy reference that you can use to improve your productivity.

## Table of Contents

- [Initializing a Repository](#initializing-a-repository)
- [Managing Files](#managing-files)
- [Committing Changes](#committing-changes)
- [Viewing Changes](#viewing-changes)
- [Undoing Changes](#undoing-changes)
- [Branching and Merging](#branching-and-merging)
- [Collaborating](#collaborating)
- [Advanced Usage](#advanced-usage)
- [Stashing Changes](#stashing-change)
- [Tagging Releases](#tagging-releases)
- [Configuring Git](#configuring-git)

### Initializing a Repository

| Command                | Description                                 |
| :--------------------- | :------------------------------------------ |
| git init               | Initializes a new Git repository.           |
| git clone <repository> | Makes a copy of an existing Git repository. |

### Managing Files

| Command                      | Description                                               |
| :--------------------------- | :-------------------------------------------------------- |
| git add <file>               | Adds a file to the staging area.                          |
| git add -p                   | Interactively add portions of a file to the staging area. |
| git add .                    | Adds all new and modified files to the staging area.      |
| git rm <file>                | Removes a file from the staging area and the file system. |
| git mv <file> <new_location> | Moves a file in the file system and stages the change.    |

### Committing Changes

| Command                 | Description                                      |
| :---------------------- | :----------------------------------------------- |
| git commit              | Creates a new commit with the staged changes.    |
| git commit -a           | Commits all modified files, including deletions. |
| git commit -m "message" | Commits with a message describing the changes.   |
| git commit --amend      | Modifies the most recent commit.                 |

### Viewing Changes

| Command           | Description                                                                     |
| :---------------- | :------------------------------------------------------------------------------ |
| git diff          | Shows differences between commits, the staging area, and the working directory. |
| git diff --staged | Shows differences between the staging area and the most recent commit.          |
| git diff <commit> | Shows differences between a commit and the working directory.                   |
| git log           | Shows the commit history.                                                       |
| git log --oneline | Shows the commit history in a condensed format.                                 |
| git log --graph   | Shows the commit history in a graph format.                                     |

### Undoing Changes

| Command                    | Description                                                       |
| :------------------------- | :---------------------------------------------------------------- |
| git reset <file>           | Unstages a file, but leaves the changes in the working directory. |
| git reset --soft <commit>  | Resets to a commit, but leaves changes staged.                    |
| git reset --mixed <commit> | Resets to a commit, unstages changes.                             |
| git reset --hard <commit>  | Resets to a commit, discards changes.                             |
| git checkout -- <file>     | Discards changes in the working directory.                        |
| git revert <commit>        | Reverts the changes made in a commit, creating a new commit.      |

### Branching and Merging

| Command                      | Description                                                                            |
| :--------------------------- | :------------------------------------------------------------------------------------- |
| git branch                   | Lists all branches.                                                                    |
| git branch <branch>          | Creates a new branch.                                                                  |
| git branch -d <branch>       | Deletes a branch.                                                                      |
| git checkout <branch>        | Switches to a different branch.                                                        |
| git checkout -b <new_branch> | Creates and switches to a new branch.                                                  |
| git merge <branch>           | Merges changes from the specified branch into the current branch.                      |
| git merge --no-ff <branch>   | Forces a new commit to be created during a merge, even if fast-forwarding is possible. |
| git cherry-pick <commit>     | Applies the changes made in a commit to the current branch.                            |

### Collaborating

| Command                       | Description                                                  |
| :---------------------------- | :----------------------------------------------------------- |
| git remote add <name> <url>   | Adds a remote repository.                                    |
| git remote -v                 | Lists the remote repositories.                               |
| git fetch <remote>            | Downloads commits, files, and refs from a remote repository. |
| git pull <remote> <branch>    | Downloads commits and merges them into the current branch.   |
| git push <remote> <branch>    | Uploads commits to a remote repository.                      |
| git push --tags               | Uploads all tags to the remote repository.                   |
| git tag                       | Lists all tags.                                              |
| git tag -a <tag> -m "message" | Creates an annotated tag.                                    |
| git tag -d <tag>              | Deletes a tag.                                               |

### Advanced Usage

| Command                    | Description                                                         |
| :------------------------- | :------------------------------------------------------------------ |
| git stash                  | Temporarily saves changes that are not ready to be committed.       |
| git status                 | Shows the status of the working directory, including any conflicts. |
| git diff <branch> <branch> | Shows the differences between two branches.                         |
| git merge --abort          | Aborts a merge that has conflicts.                                  |
| git mergetool              | Opens a merge tool to resolve conflicts.                            |
| git add <file>             | Marks a conflicted file as resolved.                                |
| git commit                 | Creates a new commit with the resolved conflicts.                   |

### Stashing Changes

| Command         | Description                                             |
| :-------------- | :------------------------------------------------------ |
| git stash       | Stashes changes in the working directory.               |
| git stash apply | Applies the most recent stash to the working directory. |
| git stash list  | Lists all stashes.                                      |
| git stash drop  | Deletes the most recent stash.                          |

### Tagging Releases

| Command                       | Description                              |
| :---------------------------- | :--------------------------------------- |
| git tag                       | Lists all tags.                          |
| git tag <tag>                 | Creates a new tag.                       |
| git tag -a <tag> -m "message" | Creates an annotated tag with a message. |
| git push --tags               | Uploads all tags to a remote repository. |

### Configuring Git

| Command                                               | Description                                                               |
| :---------------------------------------------------- | :------------------------------------------------------------------------ |
| git config --global user.name "Your Name"             | Sets the user name for all repositories.                                  |
| git config --global user.email "youremail@domain.com" | Sets the email address for all repositories.                              |
| git config --global color.ui auto                     | Enables colored output in the terminal.                                   |
| git config --global core.editor <editor>              | Sets the default text editor for Git.                                     |
| git config --global core.autocrlf true                | Converts line endings to the appropriate format for the operating system. |

## Contributing

We welcome contributions to the Git Cheat Sheet from anyone in the community. If you have any suggestions or improvements, please feel free to submit a pull request. Your contributions will help make this cheat sheet even more valuable for all Git users.

## Acknowledgements

We would like to thank all the contributors who have helped make this cheat sheet possible. Your hard work and dedication are greatly appreciated!
