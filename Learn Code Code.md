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

### Using Git

1.	Add & Commit
	You can propose changes (add it to the **Index**) using  
	```bash
	git add <filename>
	```
	or
	```bash
	git add *
	```  
	To commit these changes use  
	```bash
	git commit -m "Commit message"
	```
	Now the file is committed to the **HEAD**, but not in your remote repository yet.

2.	Pushing Changes
	Your changes are now in the **HEAD** of your local working copy. To send those changes to your remote repository, execute
	```bash
	git push origin master
	```

## Miniconda

### Install Miniconda

1.	Download [Miniconda](https://docs.conda.io/en/latest/miniconda.html#linux-installers)

2.	Bash the installer
	```bash
	bash Miniconda3-latest-Linux-x86_64.sh
	```
	
3.	Update
	```bash
	conda update conda
	```

### Managing Environments

1.	Create a new environment.
	```bash
	conda create --name my_enviroment_name
	```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwNjE0MDMzNDEsMTg0MTcyMjA3OCwxMD
U0ODIyMDIyLC05MTkxNjY0NzgsLTIyNTYzNzI2Nl19
-->