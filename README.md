git --version 

# adding user

git config --list 

git config --global user.name 'username'

git config --global user.email 'email'

# First online repo then local repo

git clone 'get online repo'

# Add and Commit

git add file_names
git add . // for all

git commit -m "some message" -m "description" 

git remote set-url origin https://<TOKEN>@github.com/TheLazyBusyCoder/someRepo.git

git push origin main

# Shifting our local repo to online repo

ls -a // to check if its git repo

git config --global init.defaultBranch main // to change the default branch name when i create new git repo localy

git branch -m main  // to rename the branch name to main

// here first create a repo on github without readme.md file

git remote add origin 'link.git'  // adding new remote (github repo)
  - remember the bug with pasting the link , just do it with mouse

git remote -v // to check the current remote repo

git remote remove origin // to remove the origin

git push -U origin main // sortcuts , in future if we write git push , it will push to origin main

# Work flow

Create github repo -> clone it -> changes -> add -> commit -> push

# Branching
  - it is used so that multiple developer can work on single project at a time. 
  - At any time we can merge the brancher

git branch // to see the current branch 

git branch -m new_name // to rename  the branch

git checkout branch_name // for navagating from one branch to another

git checkout -b new_branch_name // create a new branch

git branch -d branch_name // to delete 
  - before doing this we have to go out of the branch we are deleteing 

git push origin feature1  // created new feature1 branch -> made some changes -> commited it -> push to remote repo to a new branch 

# Merging code 
1. cli 

git diff main // comparing 2 branches 

git merge main

2. pull request
  - it lets you tell others about the changes you've pushed to a branch in a git repo 

// we do this on git hub

# Reflect online changes to your local repo 

git pull origin main 
  fetch and download online repo and match it

# Resolving merge conflicts 

// in vs code

git merge main // i am in feature1 branch 
  - it happens only when changes are on sam line. 


# undoing changes 

1. add but not commited 
  - changed the file and added , but not commited 

git reset filename.html

2. undoing commit changes

git reset HEAD~1
  - One undo 
  - HEAD is a pointer to git commites , head is lates , ~1 is -1 

git log // check the commit 

git reset commit_hash_code

git reset commit_hash_code --hard  // so it reflects the file. 

# Fork
  - rough copy of a repo 


