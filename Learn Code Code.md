# Learn Code Code

> David Ramsay

## System

[Zorin OS](https://zorin.com/os/)

## Git & GitHub

### Install Git
1.	Install
	```bash
	apt install git
	```
1.	Setting your Git username for _every_ repository on your computer
	```bash
	git config --global user.name "davidjpramsay"
	```

1.	Setting your commit email address in Git
	```bash
	git config --global user.email "david.jp.ramsay@me.com"
	```
### Connect to GitHub

1.	Generate a new SSH key
	```bash
	ssh-keygen -t ed25519 -C "david.jp.ramsay@me.com"
	```

2.	Start the ssh-agent in the background.
	```bash
	eval "$(ssh-agent -s)"
	```
3.	Add your SSH private key to the ssh-agent
	```bash
	ssh-add ~/.ssh/id_ed25519
	```
4.	Add public SSH to GitHub in the account settings menu.

5.	Clone  a repository on GitHub locally.
	```bash
	git clone git@github.com:davidjpramsay/learncodecode.git
	```
## add & commit

You can propose changes (add it to the **Index**) using  
`git add <filename>`  
`git add *`  
This is the first step in the basic git workflow. To actually commit these changes use  
`git commit -m "Commit message"`  
Now the file is committed to the **HEAD**, but not in your remote repository yet.

## pushing changes

Your changes are now in the **HEAD** of your local working copy. To send those changes to your remote repository, execute  
`git push origin master`
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE3NjQ5NTk1NjAsMTg0MTcyMjA3OCwxMD
U0ODIyMDIyLC05MTkxNjY0NzgsLTIyNTYzNzI2Nl19
-->