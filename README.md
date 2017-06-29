# Working Directory
- Area where all of our files and directories and changes are living all the time

# Staging Area
- Files and directories that we explicitly add to the staging area

# Git Repository
- Where all our snapshots are stored

# Shortcuts

- CTRL + K clears console

# Commands

## Basics

- git init: sets up git in the directory
- git status: shows current status and added/not added files
- git add <filename>: adds files to staging area
- git commit -m "message": commits the changes
- git log: shows a log of the recent commits

## Adding Files 

- touch .hidden.txt : creates a hidden file
- ls -a : shows all files, including hidden
- git add -A : add all files, including hidden ones
- git add *.html : adds all html files. * is a wildcard
- q : quit the git log "pager"

## Removing Files

- git reset HEAD file2.txt : removes a file from the staging area

## Ignoring Files

- create .gitignore file (which is hidden)
- add files to ignore to this file

# Git Branches

- git branch : list all branches
- git checkout -b <branch_name> : create a new branch
- git checkout <branch_name> : check out an existing branch
- git merge <branch_name> : merges branch into current branch. If merging into master, checkout master first!
- git branch -d <branch_name> : removes a branch

## Checking out Old Commits

- git checkout <hash of commit> : hash comes from git log, use this to go back to a prior commit
- git checkout master : gets you back

## Connecting to github

- git remote add origin <url> : adds the repository at url as origin
- git remote -v : lists remote repositories
- git push -u origin master : push to the remote repository. -u tells git to remember parameters, so all we need is "git push" next time
- git fetch origin : gets the latest version of the repository from the remote
- git merge origin <branch name> : merges the latest version of the repository with your version
- git pull origin <branch name> : performs the previous two operations together

## Other useful things

- mv oldFilename newFilename : this will rename a file (or move it if into a different directory)