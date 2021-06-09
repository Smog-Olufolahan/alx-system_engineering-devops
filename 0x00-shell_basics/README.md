
# Shell Basic Commands
* A script that prints the absolute path name of the working directory: pwd
* A script that display the contents list of your current directory: ls
* A script that changes the working directory to the user's home directory: cd
* A script that display current directory contents in a long format: ls -l
* A script that display directory contents, including hidden files (starting with .): ls -l -a
* A script to display current directory contents, long format, with user and group IDs displayed numerically and hidden files: ls -lna
* A script that creates a directory named holberton in the /tmp/ directory: mkdir /tmp/holberton/
* A script to move the file betty from /tmp/ to /tmp/holberton directory: mv /tmp/betty /tmp/holberton/
* A script to delete the file betty: rm /tmp/holberton/betty
* A script to delete the directory holberton that is in the /tmp directory: rmdir /tmp/holberton
* A script that changes the working directory to the previous one: cd -
* A script that lists all files in the current directory and the parent of the working directory and the /boot directory in long format: ls -l -a . .. /boot
* A script that prints the type of the file named iamafile: file /tmp/iamafile
* A script to create a symbolic link to /bin/ls, named __ls__: ln -s /bin/ls __ls__
* A script that copies all the HTML files from the current working directory to the parent of the working directory: cp -n -u *.html ..
* A script that moves all files beginning with an uppercase letter to a directory: mv [[:upper:]]* /tmp/u
* A script that deletes all files in the current working directory thta end with the character ~ : rm *~
* A script that creates the directories: mkdir -p welcome/to/holberton
* A script that list all the files and directories of the current directory, separated by commas: ls -map