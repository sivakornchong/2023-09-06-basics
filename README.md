# 2023-09-06-basics

Two ways to initialize git
	1. Git init then sync to the github level
	a) Git init -> this create the .git folder, turning the current folder into a git repo.
		a. Type this once per folder structure, you don't want to nest this. This is because git takes a snapshot of the whole folder structure at that point in time. 
	b) Git status 
	
	2. There is already a github repo, just clone down
	Git clone online_directory

Create snapshots (commits)
	- Adding will go into the staging area.
	- When committing a snapshot, git will search for .gitconfig file from the global setting (home dir), and uses the information. Commit means commit to memory and you can retrace etc.

	1. Git add file
	2. Git commit or git commit -m "txt"
		a. You can write the message in the file COMMIT_EDITMSG, and close it.
		b. Otherwise -m will do just fine.

To revert
Git restore to unstage (added but have not committed)

Checks
Git log 
	- will be able to find the past commit history.
	- If you don’t get your prompt back, press the letter 'q', you will see a colon on the bottom left of the terminal that indicates you need to do the 'q.'


Syncing to the remote commands
	- This will push to the remote repository (e.g. github, bitbucket, gitlab)
Git remote add origin git@github.com:sivakornchong/2023-09-06-basics.git
Git push -u origin main

Whole remote repository address = origin
/main = the branch
