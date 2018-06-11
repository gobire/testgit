Ths is for playing with git commands and effects from simple to advanced levels.

#Start by signing up and creating repository on Github

#On your local machine (I'm currently on Windows PC) ensure you have downloaded git and git Bash (terminal) is ready

#Type -->  git --version  #to get installed git version

--> git --help  #displays git key commands with explanation - help file

#Let us create a directory / repository / folder in our local machine with same name as the github repo

--> mkdir ~/testgit	#this is terminal command,  ~/ is to locate directory a level below in root directory

--> cd testgit    	#change directory to our newly created directory

## It is time to initialize git in our folder so that git can start tracking activities in the folder

--> git init		# git initialized in the directory. This adds a hidden folder /.git

## We need to tell git our identity : name and email for reference and proper tagging when synchronizing with our remote repo

--> git config --global user.name "bire"
--> git config --global user.email "aduwgobire@gmail.com"

#type --> git config user.name  	#to confirm name
#type --> git config user.email  	#to confirm email address

#################################
#Time to start creating files/documents etc within our working directory
################################

touch Readme.txt	#terminal command to create file called Readme.txt; You can create files using mouse.

# For us to update the remote repository (that is on github), we must "stage" and "commit" before "push"

--> git add Readme.txt  	#stage the file Readme.txt, that is, take a snapshot of the file in readiness to commit
or
--> git add .		# to stage all modified files,  the '.' notation is useful inorder to avoid typing names of all modified files.

--> git status		# to see the staged files or unstaged files as the case may be.

#now that our modifications on local directory are captured or staged by git, it is time to commit.

--> git commit -m "Add Readme.txt"	# it is important to start changes made in the commit, -m is for message followed by label in quotes
 
--> git log				#display information on commit and reference id for commit(s)
or
--> git log --oneline			#display condense information per line (less verbose)

#wow! Time to connect to remote repository on Github
#first, copy the link from the Github/repo page [https://github.com/gobire/testgit]. Ensure you copy your own link

#type --> git remote add origin https://github.com/gobire/testgit	#git is notified origin as https://github.com/gobire/testgit

#lastly, push the commits to the remote Github repository to update it

-->git push origin master	#master is the branch for now to receive the update as there is no other branch yet.

#Done and updated! It is this simple. We will look at more operations.... Time to stage (add), commit (-m "Complete beginner Git Tutorial") and push this work


