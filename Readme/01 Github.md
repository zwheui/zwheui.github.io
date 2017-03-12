### [Return to Readme](../README.md#git)
### Notes Github
================
##### Work on Github, here is a [link](http://pcottle.github.io/learnGitBranching/) to learn more on Git

<a name="basic"/>
* Basic Knowlege
	* Github host the repository for us
	* Git is version control software such as (SVN, TFS)
	* Install Git by [link](https://git-scm.com/download) and run `git --version`
	* Gitignore file to protect the information not push to the repository such as `password`
	* Simple Process of the github
		* Create a repository on github [link](https://github.com) by click `+ New Repository`
		* Public repository is free, private is toll
		* check the `Initialize this repository with a README`
		* open Mac Terminal and git command such as `git clone https://github.com/zwheui/zwheui.github.io`
	* Others
		* `Issues` can log different kind of the information by choose the `labels` on create a new issue page
		* Team work can be done by using `Branch` function
		* We can add Collaborators in the Settings of the Repository (not account setting)
		* The collaborator can use `new pull request`, tell the repository owner to merge the code

<a name="cmd"/>
* Command
	* git config 
		* git config --global user.name "Tom Zhu"
		* git config --global user.email "zwheui@gmail.com"
		* git config user.name git config user.email
	* git clone [git link]
	* git status
	* git add *
	* git commit -m "blah blah"
	* git log --pretty=oneline -2
	* git push		
		* (first time need to enter github email account and password
		* If two-factor opened, the password is a token which generated from [link](https://github.com/settings/tokens))
		* git push origin master
		* git push origin [branch name]
	* git pull
	* git branch (list all branch)
		* git branch [branch name]
		* git checkout [branch name]
		* git push origin [branch name]
		* git checkout master
	* git merge
		* git checkout master
		* git merge [branch name]
		* git branch -d [branch name]			(Delete a branch local)
		* git branch -D [branch name]   		(Delete a branch without merge)
		* git push orgin --delete [branch name]	(Delete a branch from Github website)

<a name="gui"/>

* Graphical UI
	* Download [link](https://desktop.github.com/) for both Mac and window
	* Not able to: 
		* Merge branch to master
		* Delete branch


<a name="md"/>

* GitHub Flavored Markdown (Chinese Link)
	* If you want to learn how to write pretty format of the *.md file such as `README.md`, learn Markdown
	* Edit:		https://github.com/guodongxiaren/README/edit/master/README.md
	* Preview:	https://github.com/guodongxiaren/README/blob/master/README.md

<a name="2f"/>

* Open the two-factor
	* In the github home page, login your account -- right click your user logo on the top right -- Settings -- Security
	* Need to install a mobile app called `Due Mobile`
	* Use the 'Due Mobile' scan the barcode, next time if you need login account again, you need to get the code from the `Due Mobile` app

* Help links:
	* Git flow vs Github flow			[link](http://lucamezzalira.com/2014/03/10/git-flow-vs-github-flow/)
	
