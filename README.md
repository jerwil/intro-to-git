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


## Other useful things

- mv oldFilename newFilename : this will rename a file (or move it if into a different directory)