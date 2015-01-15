# Basic Git Workflow:

## Vocab:
- Repo: short for repository
- Local: your personal computer
- Remote: your github repo

## Your tools:
	- git clone repository_url
		- copies a repo down to your computer
	- git pull origin branch_name
		- brings your local branch up to speed with the remote branch
	- git checkout branch_name
		- switches you to another branch
	- git checkout -b branch_name
		- creates a new branch and switches you to it
	- git status 
		- gives you a little printout showing the branch you're on, and a list of all staged/unstaged changes you've made
	- git add .
		- adds all changed files in your working directory to the stage, so that they can be committed.
	- git commit -m "your message"
		- saves all staged changes locally, making them forever a part of your git history
	- git push origin branch_name
		- updates your remote branch with all committed changes you have made locally
	- subl . 
		- opens everything in your current directory with sublime
	- git help
		- gives you a list of git commands and their functionality, in case you forget

## Your workflow:

### Setup

#### Don't have a copy of the repo on your computer yet?
- in terminal, navigate to wherever you'd like to store the repo
- run: git clone repository_url
- cd into your new repo
- run: git checkout -b new_branch
- run: subl .

#### Already have a copy?
- in terminal, cd into your repo's folder 
- run: git checkout master
- run: git pull origin master
- run: git checkout existing_branch ORRRR git checkout new_branch
- run: subl .

### Work
- in sublime, add code, change code, etc.
- git add . 
- git commit -m "a concise msg explaining any changes made"
- repeat until finished working. use git status to verify that changes and additions actually happen.

### Wrap Up
- git push origin branch_name
- make a pull request on github