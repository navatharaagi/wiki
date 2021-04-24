
# Every Day Git Commands 
* Init 
  ```
  # Create an empty git repo or reinitialize an existing one
  $ git init 
  ```
* Clone 
  ```
  # Clone repo into to specific directory
  $ git clone <repo_url> <to_directory>
  # Clone specific branch
  $ git clone -b <branch_name> <repo_url>
  # Clone a certain level of history’s depth
  $ git clone -depth=<depth_level> <repo_url>
  ```
* Branch 
  ```
  # Create New Branch 
  $ git branch <branch-name>
  # View Branches Local 
  $ git branch or $ git branch --list
  # View Remote 
  $ git branch -r or $ git branch -a (Remote and local)
  # Delete Local Branch 
  $ git branch -d <branch-name>
  # Delete Remote branch from local 
  $ git push origin --delete <branch name>
  ```
* Checkout 
  ```
  # Checkout Existing Branch 
  $ git checkout <branch name>
  # Create and Checkout Branch 
  $ git checkout -b <branch name>
  ```

* Status 
  ```
  $ git status
  ```

* Add
  ```
  # Add file/folder to staging area
  $ git add <file/folder>
  # Add all files/folders in all the folders of the repository
  $ git add . or $ git add -A
  # Add only tracked files/folders
  $ git add . -u
  ```
* Commit 
  ```
  # Commit with message 
  $ git commit -m "<COMMIT MESSAGE>"
  # Stage Tracked files and Commit 
  $ git commit -am "<COMMIT MESSAGE>"
  ```
* Push 
  ```
  # First time 
  $ git push --set-upstream origin <branch>
  $ git push
  or 
  $ git push -u origin <branch_name>
  # Push 
  $ git push origin HEAD 
  # -f as optional flag to force it
  # Push all branches and tags 
  $ git push origin --all --follow-tags 
  ```
* Pull / Fetch 
  ```
  $ git pull <remote>
  ```
* Merge / Rebase (Integrate changes) [merging-vs-rebasing](https://www.atlassian.com/git/tutorials/merging-vs-rebasing)
  ```
  # Merge the master branch into the feature branch
  $ git merge feature master
  # Rebase 
  $ git checkout feature
  $ git rebase master
  ```
* Revert (Undo Commits )
  ```
  $ git revert <COMMIT ID(SHA)>
  ```
  
# Git Global Config 
```
# First time setup 
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
# Configure Git to always push using the current branch name. 
$ git config --global push.default current
```

# To-DO 

* Rebase / Merge 
* Cherrypick 
* Reset 
* Squash 
* Revert 
* Git Config 
* Bisect 
* Git diff 
* Blame 
* Gitignore 
  
# Branching Models 
* Git Flow 
* Github Flow
* Trunk Base Development 
* GitLab Flow 
* One Flow 
* Feature Branch Flow  