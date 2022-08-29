# Git Basics

What is Git?
- The Git is an open Sourced version on control system

What is version control?
- The version control is a management of changes to the organizations files, documents, computer programs or large websites and other information.
- Here we save an initial version of the repository and update the changes made on the repository.
- Having a version control system can help to stream line the process and identify the changes and updates that are made on the files.


## Terminologies used in Git and their meaning
Directory --> Folder
Terminal --> Interface for text command
CLI --> Command line Interface
cd --> Change of directory
repository --> Project or the folder where the project files are kept.
Github --> A website that host the repository remote.

### Common Git Command 
clone --> bringing the repository hosted in same websites like Github into a folder on a local machine.
add --> Command helps to track the changes to git
commit --> Saving the file to the git
push --> uploading the commits to the remote repository.
pull --> Download the changes made from remote repository to your local pc.


On the Github the changes made can be seen commits section on github.

## Cloning a repository
This command can be used download the repository to the local machine to a given path. 

Command to use - `git clone`
how to use it - `git clone <link>`

Add the link at the end of git clone command so once git will clone the repository from given link `https://github.com/Kishores2801/My-Weekly-Datascience-Learning.git`


## Tracking the files in the repository
Before making a commit always we need to track the changes that are made documents.

To get a snapshot of repository in local machine
Command to use - `git status`

This command will give the changes that are tracked and untracked in the repository.

To track the files 
Command to use - `git add`

how to use it - `git add .` this command can be used to track all the changes made on the repository.
how to use it - `git add <file_name>`  this command allows only add particular files.

## Saving the changes made on git
The changes can be added to the git remote repository.
Command to use  - `git commit`

-m - command used for messages (what or why the changes made)

-m can be used in command twice.
    -m (first m can be used for commit message)
    -m (second m can be used for description message)

how to use it - `git commit -m "your message" -m "description"`

## Pushing the changes to github
To push the file we need to use these command
Command to use  - `git push`

how to use - `git push orgin main`
how to use - `git push <your link>`

to  make the path to push as default

how to use - `git push -u orgin main`
how to use - `git push -u <your link>`

## creating a repository locally

To initialize a git repository locally
Command to use  - `git init`

To add remote repository to locally
command to use - `git remote add orgin <your_link>`

To check whether the file is connected
command to use - `git remote -v`


## Git Branching
The branching process can help to keep the changes separate which can be used to add when adding new features and test those features. once the testing is finalized the branch can be merged.

To check the current branch you are on
command to use - `git branch`

To create a new branch in repository
command to use - `git checkout -b feature <branch_name>`

Merging a feature branch/ hotfix branch with main branch
command to use - `git merge <branch_name>`

## Undoing a change made
command use - `git reset`

to undo a commit made
command use - `git reset HEAD ~1`

We can also revert the change made to previous change made by giving the referral hash value for commit as
To get the value hash values
command to use - `git log`

and then give `git reset --hard <SHA-1>`