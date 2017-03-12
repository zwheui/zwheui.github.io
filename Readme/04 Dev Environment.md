### [Return to Readme](../README.md#devenv)
### Notes Dev Environment
================
##### Here are the steps to build develop environment on MAC OSX

* If you don't have a MAC, use VMWare to install OSX, the install file is on the Company file server 8.19
* Don't learn Ruby on rails on windows, windows is not fully supported by Ruby
* Ruby version management such as RVM or rbenv is only available in Linux OS


<a name="steps"/>

* Steps
	* Install XCode from App Store
	* run gcc -v
	* run which gcc
	* run which make

* Homebrew [link](http://brew.sh/)
	* Goto the home of Homebrew and copy the install command and run in the terminal 
	* brew doctor
	* brew update

* Ruby version 2.3.0

<a name="rbenv"/>
* How to in (Chinese) [link](https://segmentfault.com/a/1190000000366488)
* brew install rbenv
* nano .bash_profile		eval "$(rbenv init -)"
* source ~/.bash_profile
* which rbenv
* ruby -v
* rbenv install 2.3.0 					(install ruby)
* rbenv shell/local/global 2.3.0		(switch ruby version, the `shell` mean the terminal session, the `local` mean the folder)
* rbenv versions 						(list all ruby versions)
* rbenv rehash

<a name="gem">

* gem -v
* which gem
* gem list					(list all gems installed)
* gem update --system		(be careful, since this is the first time we config dev environment, it's OK)

<a name="bundler"/>

* gem install bundler
* rbenv rehash
* bundle -v
* which bundle

<a name="rails"/>

* gem install rails --no-ri --no-rdoc
* rails new (Demo01)
* cd Demo01
* rails s 					(Start the webrick)
* open browser and put http://localhost:3000
