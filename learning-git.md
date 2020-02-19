# Git Explained
## Version Control
A system that allows you to view/revert to previous versions of a file by recording changes that are made/who made the changes.
### Local Version Control
One database on your hard disk that stores changes to files.
### Centralized Version Control
A single server that stores all changes and file versions that can be accessed by various different people.
### Distributed Version Control
Creates mirrored repos -backups- to replace any lost info in the case of the CVCS failing and losing data.
## What is Git?
### Snapshots
A form of DVCS, where whenever you commit your project, Git creates a snapshot of the current version and stores all changes to the info.
### Local Operations
Stores project history on the local disk, which eliminates the need for internet or a server to work on a project.
### Tracking Changes
Git tracks all changes and detects possible loss of information.
### Loss of Data
Git makes it difficult for a snapshot to be lost, protecting against irreversible damage.
### States
The three main states of files:
* Committed
    * Data is stored locally.
* Modified
    * File has been changed, but not committed.
* Staged
    * File is flagged to be committed.  
## History of Git
Git began with the open source software, Linux kernel, when the devs began using the BitKeeper DVCS. In 2005, tensions between the dev team and the BitKeeper company lead to the cessation of their usage of BitKeeper and the beginning of the development of Git by the chief architect, Linus Torvalds.
## Customization
### Configuration of Variables
Use the command `git config` to configure variables altering the operation and look.
## Default Text Editor
Git will use the system's default editor until you use the command `git config --global core.editor /name of text editor/`
## Check Settings
To check settings, use `git config --list`
## Getting Help
There are three ways to get info on any command
* `git help /command/`
* `git /command/ --help`
* `man git-/command/`  
## Setting up a Git Repository
### Importing
To import an existing project into Git:

1. Switch to the project directory
2. Use the `git init` command
3. To start tracking, perfome an initial commit using the commands
    * `git add *.c`
    * `git add /license/`
    * `git commit -m "/message/"`  
Now the files are being tracked and have an initial commit  
### Cloning
You can create a copy of an existing repo by using the command `git clone /repo URL/`  
Cloning creates a copy of all versions of all files in a project. It creates a directory with an initialized .git directory inside, containing all the copies. The command will also chek/retrieve the newest version of the project.  
To create it with a chosen name rather than the default, use the command `git clone /repo URL/ /chosen name/`
## Workflow
### Local Repository Structure
The local Git repo has three components:  
* Working Directory
    * Where the files reside
* Index
    * The area used for staging
* Head
    * Point to the most recent commit

### Saving Changes
All files in a checked out -working- copy of a file are either
* Tracked
    * Can be modified, unmodified, or staged - most recent file snapshot
* Untracked
    * Not in the last snapshot and do not reside in the staging area

### The Life Cycle of File Status
* Git flags files as modified after a change has been made since the last commit
* The modified file is staged
* The staged changed are committed

### Check File Status
To determine the state of files, use the command `git status`
### Tracking and Staging a New File
* Single File
    * Track only one file using the command `git add /filename/`
* All Files
    * Track all files using the command `git add *`
    
### Committing a File
After staging one or multiple files, the changes should be committed with a commit message using the command `git commit -m "/message explaining changes/"`
### Committing All Changes
Commit a snapshot of all modifications to tracked files with the command `git commit -a`
### Pushing Changes
After committing, you push the changes to the remote origin repo from your local master branch using the command `git push origin master`
### Stashing Changes
When you aren't ready to commit changes, but don't want them to be lost, temporarily remove and hide the changes with the command `git stash`  
When you want to continue working with them, retrieve them with the command `git stash apply`
## Remote Repositories
Teams can use remote repos -versions of a project residing online- to collaborate, push info, and pull data. You can work with multiple repos that can be assigned read/write or read-only privileges.
### Cloned Repositories
For cloned repos, the server from which the clone was made will be named 'origin' and your branch will be called 'master.'
### Seeing Your Remotes
You can view the names -like origin- of all specified remote handles next to their URLs with the command `git remote -v`

[back](README.md)