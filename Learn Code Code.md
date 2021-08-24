# Learn Code Code

> David Ramsay

## System Setup

![](https://raw.githubusercontent.com/davidjpramsay/learncodecode/master/images/zorin-logomark-blue.png =65x)
[Zorin OS](https://zorin.com/os/)


### Git & GitHub

#### Install Git
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
#### Connect to GitHub

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

#### Using Git

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
3.	Check status.
	```bash
	git status
	```

### Miniconda

#### Install Miniconda

1.	Download [Miniconda](https://docs.conda.io/en/latest/miniconda.html#linux-installers)

2.	Bash the installer
	```bash
	bash Miniconda3-latest-Linux-x86_64.sh
	```
	
3.	Update
	```bash
	conda update conda
	```

#### Managing Environments

1.	Create a new environment.
	```bash
	conda create --name my_enviroment_name
	```
2.	Activate environment
	```bash
	source activate my_enviroment_name
	```
3.	List all environments
	```bash
	conda info --envs
	```
4.	Change back to base.
	```bash
	conda activate
	```
5.	Install packages.
	```bash
	conda install python numpy pandas jupyterlab
	```
6.	List packages in environment.
	```bash
	conda list
	```
7.	Delete environment.
	```bash
	conda remove --name my_environment_name --all
	```

### Jupyter

1.	Launch JupyterLab
	```bash
	jupyter-lab
	```

## Learn Python

1.	[Learn Python - Full Course for Beginners [Tutorial]](https://www.youtube.com/watch?v=rfscVS0vtbw&t=0s)
2.	[Automate the Boring Stuff with Python](https://automatetheboringstuff.com/)

## ML Courses

1.	[Coursera - Machine Learning](https://www.coursera.org/learn/machine-learning)
2.	[Coursera - Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning)
3.	[Practical Deep Learning for Coders](https://course.fast.ai/)
4.	[Part 2: Deep Learning from the Foundations](https://course19.fast.ai/part2)

## Resources

1.	[arXiv](https://arxiv.org/)
		
3.	[Mathematics for Machine Learning](https://mml-book.github.io/book/mml-book.pdf)
4.	[Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/index.html)
5.	[Deep Learning](https://www.deeplearningbook.org/)
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTExOTUyNTQyNTEsNjkyMjY0MDY5LC0xNT
k2NjkzMDgwLC0xODI1MTMyOTIxLC00MDIyMzg2NzYsLTY3NDMx
NTgyMSwtMTkxOTU3Njg5NywtMTkxOTU3Njg5NywxNjc1NTc1MD
kwLC02NTk5Njk3NjAsLTI3MzQ3MTc3LC0xNTUxNTY1OTU2LC0y
MDE2MjE2MjI4LDE4NDE3MjIwNzgsMTA1NDgyMjAyMiwtOTE5MT
Y2NDc4LC0yMjU2MzcyNjZdfQ==
-->