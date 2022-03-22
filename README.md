# Github and Git core commands I need

Here I discussed about github and git core commands that are using regulary.

## Officila Git Documentation

## For Git Initialization (the very first step )

git init

## Cloning a git repository

git clone <link_here>

## Stage All Changes

### For staging all files and folder inside the parent folder

git add --all

### same as git add --all

git add --A

### This command will stage all files only inside the working directory. So, this command is recommended to use inside the parent directory

git add .

### if i delete a file or folder from a staged files or folder , this command will not stage the deleted file or folder

git add \*

### this command will stage all files with the same extension name

git add \* .filesExtension

### reset all staged commands

#### for reset all command we've done and it will return only changes not the deleted files

git reset

### git reset with deleted files

#### like we deleted a file and want to also reset to change stating then we will use this command and it will roll back the file and stage

git reset --hard

### recommended is to use git add . from the parent directory

#### to upload or commit in the local repository

git commit -m "summary of your changes to the files"

### reset all commited commands

#### if I undo all commands after commiting and want to go to staging format

git reset HEAD~

### remove or delete a file using git command

#### this command will delete the selected file and also stage the changes.

git rm filesname.extension

### remove a file forcefully

#### this command will delete the files even if i change anyting in that particular file.

git rm filesname.extension -f

### chached files

#### this command will not delete the file but update to the staging directory

git --cached filesName.extension

### remove all folder inside all folder

#### this command will delete the parent folder inside all folder

git rm -r <foldersName>

### git branch

#### will show you how many branch are there and which branch you are in

git branch

### make a new branch

#### will make a new branch

git branch <brnachName>

### go to the other branch

#### will take you to your choosing branch

git branch checkout <brnachName>

If you want to merg branches, you must checkout other branch always commit the code.
//margin with other branch
git marge main -m "comment" --------- to merge a branch with main branch you should use this git command and you must checkout the branch from main branch

=================================================
push codes to remote repositor
=================================================

git push origin <brnachName> (to send the code at remote repository )

=================================================
If you are sure your local master has the latest changes you want on remote, then do git push --force
=================================================

git push --force origin <brnachName>

=================================================
The git set-upstream allows you to set the default remote branch for your current local branch. By default, every pull command sets the master as your default remote branch.
=================================================

git push --set-upstream origin main

=================================================
change the git branch name
=================================================

git branch --move <currentBranchName> <theBranchName_you_want_to_set>

=================================================
delete git branch from the remote repository
=================================================
This command will show you the branhes that are in remote repository

git branch --all

After git branch --all command you will see the branches from the remote repository and you can delete the branch with below command

git push origin --delete <branch_name_you_want_to_delete>

++++++++++++++++++++++++++++++++++
hello world++++++++++++++++++++++++

---
