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
### Connect to GitHub with SSH

1.	Generate a new SSH key
	```bash
	ssh-keygen -t ed25519 -C "david.jp.ramsay@me.com"
	```

1.	Start the ssh-agent in the background.
	```bash
	eval "$(ssh-agent -s)"
	```
1.	Add your SSH private key to the ssh-agent
	```bash
	ssh-add ~/.ssh/id_ed25519
	```
1.	Add public SSH to GitHub in the account settings menu.

1.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTc2NjAxMDQ0OSwxMDU0ODIyMDIyLC05MT
kxNjY0NzgsLTIyNTYzNzI2Nl19
-->