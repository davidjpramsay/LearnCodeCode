# Learn Code Code

> David Ramsay

## System

[Zorin OS](https://zorin.com/os/)

## Git & GitHub

### Install Git
1.	Install
	```console
	apt install git
	```
1.	Setting your Git username for _every_ repository on your computer
	```console
	git config --global user.name "davidjpramsay"
	```

1.	Setting your commit email address in Git
	```console
	git config --global user.email "david.jp.ramsay@me.com"
	```
### Connect to GitHub with SSH

1.	Generate a new SSH key
	```console
	ssh-keygen -t ed25519 -C "david.jp.ramsay@me.com"
	```

2.	Start the ssh-agent in the background.
	```console
	eval "$(ssh-agent -s)"
	```
3.	Add your SSH private key to the ssh-agent
	```console
	ssh-add ~/.ssh/id_ed25519
	```
4. Add SSH to GitHub

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIyNTYzNzI2Nl19
-->