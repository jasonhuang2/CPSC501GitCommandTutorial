# CPSC501GitCommandTutorial
CPSC 501 Git Command Tutorial through terminal commands 

Commands used in this tutorial:
To clone a repository (assuming a repo already exists in GitHub and an SSH key is already initalized):
1. On terminal, navigate to folder 
2. "git clone https://github.com/jasonhuang2/CPSC501GitCommandTutorial.git"
	- This will clone an already existing repo using HTTPS

Local repository consists of three "trees"
1. Working directory: holds actual files
2. Index: The staging area 
3. Head: points to the last commit I've made 

To update my local repository for the latest changes BEFORE YOU START CODING:
"git pull" 

To create a new branch named "feature_x":
1. git checkout -b feature_x 
2. A branch is not available to others unless I push the branch to my remote repository:
	- git push origin feature_x


To check which branch I am currently on:
1. git branch 

To switch back to another branch (ie: master):
1. git checkout master

To get the differences between branches (ie: difference between lineFeature branch and master branch):
1. git diff lineFeature master 

Assuming I'm in lineFeature branch which branched off from master. I updated a whole bunch of files and now I want to update my local repo and remote repo. If everything's working, I want to merge lineFeature to master branch! 
1. git add <filename> (THIS ADDS MY CHANGES TO INDEX)
	- git reset -- <filename> (THIS RESET CHANGES)
	- or "git add *" if you have multiple files
2. git commit -m "Your commit message goes here" (THIS COMMITS MY FILES TO THE HEAD, NOT IN REMOTE REPO YET)
3. git push origin lineFeature (THIS PUSHES MY CHANGES TO MY lineFeature BRANCH)
4.  Gratz! lineFeature branch now has all my changes! 

5. git merge master (THIS MERGES MY lineFeature branch to my master branch)


 
