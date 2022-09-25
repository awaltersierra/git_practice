# GIT COMMAND

- git init
- git status
- git log
- git add "Filename"
- git diff
- git commit -m "Comment"
- git commit --amend --no-edit (Replace the last Commit without edit the Commit Message)
- git show HEAD (show the last commit)
- git checkout HEAD filename (restore filename in local directory)

- git reset HEAD filename (restore a file on staging area, that we dont to include in the commit)
- git reset COMIT_SHA (7 digitos del SHA del commit que queremos restaurar)

## STASH
- git stash (save local work to continue work for another branch)
- git branch NAME (create a new branch)
- git checkout NAME (make you that branch)
- git stash list 
- git stash pop (bring you the stash lastone)

## ALIAS

+ $ git config --global alias.co "checkout"
+ $ git config --global alias.br "branch"
+ $ git config --global alias.glop "log --pretty=format:"%h %s" --graph"

## HOW CREATE A REPOSITORY ON THE COMMAND LINE

1. echo "# git_practice" >> README.md
2. git init
3. git add README.md
4. git commit -m "first commit"
5. git branch -M main
6. git remote add origin https://github.com/awaltersierra/git_practice.git
7. git push -u origin main

## HOW PUSH AN EXISTING REPO ON THE COMMAND LINE

1. git remote add origin https://github.com/awaltersierra/git_practice.git
2. git branch -M main
3. git push -u origin main

## BRANCHES
+ git branch: Lists all a Git project’s branches.
+ git branch branch_name: Creates a new branch.
+ git checkout branch_name: Used to switch from one branch to another.
+ git merge branch_name: Used to join file changes from one branch to another.
+ git branch -d branch_name: Deletes the branch specified.

## TEAMWORKS WORKFLOW

+ Fetch and merge changes from the remote
+ Create a branch to work on a new project feature
+ Develop the feature on your branch and commit your work
+ Fetch and merge from the remote again (in case new commits were made while you were working)
+ Push your branch up to the remote for review

### Commands

+ git clone remote_location clone_name (clone remote repo into local machine)
+ git remote -v (see the branch)
+ git fetch (fetch changes from remote 'origin' into your origin/master branch)
+ git merge origin/master (could merge the changes that bring with fetch command)
+ git push origin <your_branch_name> (push  from local machine to remote)
