### [Return to Readme](../README.md#linuxos)
### Notes LinuxOS
================
##### Here are the list of Linux OS

* In most cases Linux don't need to restart, just use `sudo apt-get update` instead.
* In most cases, Linux have only 1 disk which windows will have disk C: disk D: disk E:
* `sudo` is a command which basicly like `run as administrator` in windows
* Be careful run the command, some command such as: `sudo chown -R tomzhu:tomzhu /usr` will crash the sudo command

* Basic Command
	* sudo su
	* ll 								(List all the file and folder)
	* pwd								(Check current Path)
	* cd .. cd ~						(Change directory)
	* mkdir								(Create Folder)
	* md -rf (folder name)				(Remove folder which contain files)
	* nano (file path/file name)		(Edit file)
	* cat (file path/file name)			(Output file text)
	* echo $PATH echo 'hello world'		(Check the system environment path)
	* which (software name)				(List the path of this software)
	* find / -type f -name "index.html"	(find the file under the current folder)
	* apt-get install (software name)	(install software)
	* sudo reboot						Restart)
	* ifconfig							(Check intranet IP)
	* host myip.opendns.com resolver1.opendns.com (Check inernet IP)
	* sudo chmod -R 0755 .				(grant read and write, need to goto the folder first)
	* sudo chmod 777 .					(grant delete, need to goto the folder first)
	* sudo chown -R $(whoami) /usr/local/lib/
	* sudo chown -R tomzhu:tomzhu /etc/nginx/sites-enabled	(grant access right to certain user, not recommend to use this, be careful)
	* netstat -tulnp | grep (port no)	(Check port, if not in use, then nothing return)

<a name="ubuntu"/>

* Ubuntu
	* Use putty to remote Ubuntu by ssh
	* Use puttycm (putty connection manage) which can open putty in many tabs
	* Set Static IP [link](http://www.howtogeek.com/howto/ubuntu/change-ubuntu-server-from-dhcp-to-a-static-ip-address/)
	* Add New User Command
		* useradd -m -s /bin/bash tomzhu
		* adduser tomzhu sudo
		* passwd tomzhu

	* Add New User in AWS [link](http://www.brianlinkletter.com/how-to-set-up-a-new-userid-on-your-amazon-aws-server-instance/) 

<a name="osx"/>

* Mac OSX
	* use terminal to run command of linux, terminal is like `cmd` in windows
	* ls -la (same as ll, we can put this command in the .bash_profile)
	* MAC OS X has ruby, apache by default