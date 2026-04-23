# GIT
Everything I learned about GIT and GITHUB 

1) What is Version Control System ?
   ---------------------------------
   It is a software tool that manages two major problems - Sharing of code among multiple people and Versioning of files
   There are 2 types of Version Control System:
   
   #CENTRALIZED VERSION SYSTEM :- there is a single system where files and there version history are kept. Dev pulls code to local from cerntral system make changes                                    commit back to system.
   
   #DISTRIBUTED VERSION SYSTEM :- We can make copy of entire repo on our local, make changes, commits and merge it back to system repo.
   ####################################################################################################################################################################

2) Local Repo Setup
   ----------------
   set username and email that is common for all repo in local by:

    git config --global user.name "Your Name"
    git config --global user.email "your_email@example.com"

####################################################################################################################################################################

3) Sync Local Repo to Remote
   ---------------------------

git remote add origin <github  repo link>  ---> only required on fresh account to setup
git branch -M main ---> only required on fresh account to setup
git push -u origin main
#################################################################################################################################################################

4) How to commit changes
   ----------------------

   git add .
   git commit -m "message" 
   git push origin main (to push the changes to remote)

##############################################################################################################################################################

5) Git commands
   ------------

   * git log --> to show git commits
   * git log --oneline --> to show smaller commits
   * git show <commitid> --> to see the changes
   * git checkout <branchname> --> to switch branches
   * git checkout -b <branchname> --> to create new branch
   * git merge <nameofbranchuwanttomerge> --> to merge changes of one branch to another (make sure ypu are in the branch in which u want to merge changes)
   * git clone <url> --> to copy repo from remote to local

GIT ROLLBACK
------------
* git checkout <filename> --> to undo the changes in file, if file is not moved to staging area
* git restore --staged <filename> --> if u want to rollback file that is in staging area
* git revert HEAD --> if u have commit the file and then you want to rollback, but it will create a new commit that will be same as previous commit
* git reset --hard <comitid_of_version_u_want_to_go> 











































   
