# Committing Changes in Git and Pushing to a GitHub Repository

Some things that you need to remember about this lesson:

*Begin by creating a repo on GitHub
*After repo is created use the command "git clone <URL>" in  GitBash
    *If you are using SSH you'll have to have your key setup on your GitHub account


* cd to the newly cloned repo
* use command 'ls' to see the contents of the repo
* In the video the command 'touch <filename.extension>' was used to create a .md file
* Command 'git remote -V' shows the remote connections 
* Must stage the files in order to commit them to GitHub
	*To do this use the command 'git add <file name.extension>'
	*Additionally you can use 'git add .' to stage all of the files in the repo
* You will know that your files are ready to be committed by using the 'git status' command
* The command 'git commit' is used to commit changes
	*You must always use the arguement '-m"<enter note here>"' along with this command to provide a short description of the changes made
	*Example 'git commit -m"Changed the readme.md file"'
#Everything that has been done to this point is only affecting the local machine
* In order to push changes made to your github account use the command 'git push'
	*Example: git push origin master

#Important commands that you went over

* cd - change directory, must be accompanied by a file/folder path
	* ex. cd c:\users\jdennis\desktop
* ls - lists the contents of the current directory

* git clone - Used to clone a repo from GitHub to the local machine. Must have a https url and/or SSH url/key pair
	* ex. git clone https://github.com/jst-jdennis/teset-repo.git
	* after cloning is complete use the 'cd' command to navigate to the newly created sub-directory. It will have the same name as the repo on GitHub
* git remote -v - Allows you to see references to repo's that are not on your local machine
	* If for some reason the origin remote was not created in the cloning process be sure to add it using the command 'git remote add origin <url>'
* touch <filename.extension> - An especially handy command in windows that allows for the creation of files with non-standard filetypes
	*ex. touch new.md creates the new markdown files 'new'
* git status - Shows the status of the local branch
	*ex. in this case when I ran the git status command gitbash showed the following " modified:  README.md  "
* git add <filename.extension> - Use to stage what will be committed
	* use git add . as a wildcard for all of the files in the branch
* git commit -m"" - Once staged files are committed using this command
	* Always use the arguement '-m' to add a message about the changes being committed
* git log - Used to check whether the commit is there 
* git push origin master -  This is used to push the committed changes to our github account
	* Its saying we want to push the 'master' branch to 'origin' remote
	* We setup the 'origin' remote to refer to our github repo
