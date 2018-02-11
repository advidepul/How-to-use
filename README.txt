# How-to-use

Installing Git
https://git-scm.com/downloads

git config --global credential.helper 'cache --timeout=3600': Set the cache to timeout after 1 hour (setting is in seconds)
git remote add origin <github repository address>: add one repository on github
git remote: show existing repository
git remote -v: show more info (fetch & push)
git push <remote> <branch>: push <branch> to <remote> --> upload branch on remote
git pull <remote> <branch>: download (update) branch from remote
git fetch origin: latest origin (github) will be updated on local (git)
fork: fork other person's github page to your github page

Adding a Repository to Github:
make a repository on Github
git remote add origin <github repository address>
upload files on local (git)
git push origin master
------------------------------------------------------------------------------------------------------------------------
COMMANDS
git init: make a repository folder from a working directory
git status: show which files in working direcotry have been modified/added to staging area 
		remaining in the working directory
git add <filename>: add <filename> to staging area
git commit: add what's in staging area to repository (upload) 
git log: show hisotry(versions) of repository (press q to quit)
git clone <https://...>: clone a github page
git config --global color.ui auto: get colored diff output

MODIFYING FILES
git diff: show what has been modified after modifying files in working directory (before adding)
git diff --staged: show differences between recently committed files in repository and files in staging area
git diff <ID number> <ID number>: show differences between versions of repository
git reset --hard: reset the modification made 

UPLOADING FILES 
Make a folder for repository 
cd to the folder (file(s) to be uploaded is in the folder) 
git init
git status
git add <filename>
git status
git commit
git status
git log

working directory --> staging area --> repository

MAKING A BRANCH
git branch: show what branches are present
git branch -a: show all branches including ones on git hub
git branch <branch name>: create a branch named <branch name>
git checkout <branch name>: switch current branch to <branch name>
git log --graph --oneline <branch name> <branch name> ... <branch name>: shows log for entire branch in timeline
git checkout -b <branch name>: create and switch to the <branch name>
git merge <branch name1> <branch name2>: merge branch name2 to branch name1
git show <ID number>: show diff btwn the ID number with its parent 
git branch -d <branch name>: delete <branch name>