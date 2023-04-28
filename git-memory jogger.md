### some commonly used Git commands:

1. ```git init```: initializes a new Git repository in the current directory.
2. ```git add <filename>```: adds the specified file to the staging area.
3. ```git commit -m "commit message"```: commits the changes in the staging area with a commit message.
4. ```git status```: displays the current status of the repository, including any uncommitted changes.
5. ```git log```: displays the commit history of the repository.
6. ```git config```: to configure various aspects of the Git environment. 
7. ```git branch```: lists all branches in the repository and highlights the current branch.
8. ```git checkout <branch-name>```: switches to the specified branch.
9. ```git merge <branch-name>```: merges the specified branch into the current branch.
10. ```git push```: pushes local changes to the remote repository.
11. ```git pull```: pulls changes from the remote repository to the local repository.
12. ```git clone <repository-url>```: clones a remote repository to the local machine.
13. ```git remote -v```: lists all configured remote repositories and their URLs.
14. ```git fetch```: downloads the latest changes from the remote repository without merging them.
15. ```git cherry-pick <commit-id>```: to apply a specific commit to the current branch. 
16. ```git commit --amend```: to modify the most recent commit.
17. ```git rebase```: to reapply changes from one branch onto another. This can be used to keep a clean and linear commit history.
18. ```git stash```:  to temporarily save changes that are not yet ready to be committed. This can be useful when you need to switch to another branch or pull changes from a remote repository.
19. ```git revert```: to undo a previous commit by creating a new commit that undoes the changes introduced in the original commit.
20. ```git reset```: to undo changes by resetting the state of the repository to a previous commit.
     - ```git reset --soft```: the changes made since the specified commit are still staged and will be included in the next commit.
     - ```git reset --mixed```: the changes made since the specified commit are unstaged and will not be included in the next commit.
     - ```git reset --hard```: the changes made since the specified commit are discarded and cannot be recovered.
21. ```git tag```: to create, list, or delete tags in the repository.
22. ```git diff```: to show the changes between two versions of a file or the entire repository.
23. ```git checkout```: to switch between branches or to create a new branch.
24. ```git restore```:  to discard changes made to the working directory or staging area.
25. ```git rm```: remove files from the working tree and from the index.
26. ```git checkout -b```: create a new branch and switch to it.
27. ```git clean```:  remove untracked files from the working tree.


### Extra-topics 

28. Fork: creating a copy of a remote repository on your own GitHub account.
29. .gitignore: the ".gitignore" file is a configuration file that specifies files or directories that should be ignored by Git when tracking changes to a project.
30. PR: Pull Request (PR) is a feature that allows you to propose changes to a project that is hosted on GitHub. 

