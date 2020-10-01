Linux-Commands-Cheat-Sheet
==========================

A compilation of some commonly used Linux commands for beginners (and those of us who often just forget :))

Files & Folders
----------------

Some common commands for navigating, moving, deleting & more!

##### Navigate to a folder
	cd /path/to/folder

#####  Create a folder
	mkdir folder

#####  Create a folder, then navigate to it (One command)
	mkdir folder && cd folder

#####  Move a file or folder to another folder
	mv /path/to/file.txt /path/to/dest/
	mv /path/to/folder1 /path/to/dest/

#####  Move multiple folders
	mv folder1 folder2 /path/to/dest/

##### Display files (with details) in a folder
	ls -l

#####  Zip up a file or folder
	tar -cvzf filename.tar.gz folder/

#####  Unzip a file or folder
	tar -xvzf filename.tar.gz

#####  show hidden files
	ls -a

#####  show parent working directory
	pwd

#####  Exit to directory
	cd..

#####  To remove a blank directory.
	rmdir dirname 

#####  To Delete files
	rm filename

#####  Help at command line
	man ls

#####  make a blank file
	touch filename.txt

#####  To show currently log in user
	whoami
	
#####  To search a file at location
	find -name filename

#####  To show the partition details of hard disk
	fdisk - l

#####  To show last 1000 commands, which is stored in /root/.bash_history
 	history

#####  To logout via current user
	exit
	logout

##### 	To shutdown
	shutdown -h now
	halt
	power off

#####  To Reboot
	#reboot
	init6
	shutdown –r now
	
Transferring files
----------------

Securely (over SSH) and locally

#####  Copy a file from one location to another
	cp /path/to/file.txt /path/to/dest

#####  Copy a folder from one location to another
	cp -r /path/to/folder /path/to/dest




Permissions
----------------

For more info on types of permissions and what they mean, [go here](http://en.wikipedia.org/wiki/Chmod "Title")

#####  Change permissions of a file
	chmod 755 file.txt

#####  Change permissions of a folder
	chmod -R 755 /path/to/folder







