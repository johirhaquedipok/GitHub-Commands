git init ---------- for git initialization
git clone -------- for cloning a git repository

stage all changes
git add --all ----- for staging all files and folder inside the parent folder
git add --A ------ same as git add --all
git add . --------  this command will stage all files only inside the working directory ***.
git add * --------- if i delete a file or folder from a staged files or folder , this command will not stage the deleted file or folder
git add *.filesExtension ----- this command will stage all files with the same extension name

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

git rm filesname.extension -f    ----------this command will delete the files even if i change anyting in that particular file.

// chached files

git --cached filesName.extension   --------- this command will not delete the file but update to the staging directory

// remove all folder inside all folder

git rm -r foldersName -------- this command will delete the parent folder inside all folder

///git branch//
git branch  ------ will show you how many branch are there and which branch you are in

// make a new branch
git branch branchName  ----- will make a new branch

// go to the other branch
git branch checkout branchName ---- will take you to your choosing branch

*** before you checkout other branch always commit the code . 
//margin with other branch
git marge main -m "comment" --------- to merge a branch with main branch you should use this git command and you must checkout the branch from main branch

//