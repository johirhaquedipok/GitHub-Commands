For more to read from official git documentation : https://git-scm.com/book/en/v2/Git-Branching-Branch-Management

git init ---------- for git initialization
git clone -------- for cloning a git repository

stage all changes
git add --all ----- for staging all files and folder inside the parent folder
git add --A ------ same as git add --all
git add . -------- this command will stage all files only inside the working directory _\*\*.
git add _ --------- if i delete a file or folder from a staged files or folder , this command will not stage the deleted file or folder
git add \*.filesExtension ----- this command will stage all files with the same extension name

// reset all staged commands
git reset ----------- for reset all command we've done and it will return only changes not the deleted files

//git reset with deleted files
git reset --hard ----- like we deleted a file and want to also reset to change stating then we will use this command and it will roll back the file and stage

// recommended is to use git add . from the parent directory
git commit -m "summary of your changs to the files" ------- to upload or commit in the local repository

// reset all commited commands
git reset HEAD~ -------------- if i undo all commands after commiting and want to go to staging format

// remove or delete a file using git command
git rm filesname.extension -------- this command will delete the selected file and also stage the changes.

// remove a file forcefully

git rm filesname.extension -f ----------this command will delete the files even if i change anyting in that particular file.

// chached files

git --cached filesName.extension --------- this command will not delete the file but update to the staging directory

// remove all folder inside all folder

git rm -r foldersName -------- this command will delete the parent folder inside all folder

///git branch//
git branch ------ will show you how many branch are there and which branch you are in

// make a new branch
git branch <brnachName> ----- will make a new branch

// go to the other branch
git branch checkout <brnachName>e ---- will take you to your choosing branch

\*\*\* before you checkout other branch always commit the code .
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

## hello world
