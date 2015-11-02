Linux-Commands-Cheat-Sheet
==========================

[![Join the chat at https://gitter.im/petronbot/Linux-Commands-Cheat-Sheet](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/petronbot/Linux-Commands-Cheat-Sheet?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

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

#####  Find and replace in a file
	sed -i '' 's/old/new/g' file.ext

- `sed` = Stream EDitor
- `-i` = in-place (i.e. save back to original file)
- `old` = regex to replace
- `new` = text to replace it with
- `g` = global (i.e. replace all, not just first)


Transferring files
----------------

Securely (over SSH) and locally

#####  Copy a file from one location to another
	cp /path/to/file.txt /path/to/dest

#####  Copy a folder from one location to another
	cp -r /path/to/folder /path/to/dest

#####  Sync two folders
	rsync -a /path/to/folder /path/to/dest

- `-a` = Archive, syncs recursively and preserves sym links, special and device files, modification times, group, owner, and permissions
- Source folder can be a remote, e.g. `username@server.com:/path/to/folder`




Permissions
----------------

For more info on types of permissions and what they mean, [go here](http://en.wikipedia.org/wiki/Chmod "Title")

#####  Change permissions of a file
	chmod 755 file.txt

#####  Change permissions of a folder
	chmod -R 755 /path/to/folder







