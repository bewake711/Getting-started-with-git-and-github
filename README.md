# Getting-started-with-git-and-github
Instruction to push projects to github

To upload a project from PC, open git bash on the required project folder.

Then type,

git config --global user.name bewake711

git config --global user.email "bibekthapa143@gmail.com"

touch .gitignore       
(This makes a file where the files are to be ignored,   list the folders or file that are to be ignored eg: ".ipynb_checkpoints/")

Then type,

git init

git add .                  (dot pani ho)

git commit -m "Initial Commit"

git status
(gives status of repository)

Create a private repository in github (do no tick create readme file). CLick on SSS on repository link on github (of the created repository) and copy link, then type

git remote add origin git@github.com:bewake711/Matplotlib-Examples.git

Then,

git push origin master

This will fail as there is no authentication. For this, you should create SSH keys.
Go to account setting on github, 
	select SSH keys
	Add new SSH keys
	Generate a SSH online using githhub
	run the code given in here:        https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
	Now run the SSH key on git bash,   eg:    cat /c/Users/dell/.ssh/id_rsa.pub
	SSH key is given on bash, paste this on "add SSH key" on github

Now again do,

git push origin master

DONEEEEEE!    code will be pushed now to githhub
 


