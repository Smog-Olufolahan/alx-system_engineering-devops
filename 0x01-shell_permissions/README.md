# A repository about shell permission commands
## 0. My name is Betty
* A script that switches the current user to the user betty: su betty
## 1. Who am I
* A script that prints the effective username of the current user: whoami
## 2. Groups
* A script that prints all the groups the current user is part of: groups
## 3. New owner
* A script that changes the owner of the file hello to ther user betty: chown betty hello
## 4. Empty!
* A script that creates an empty file called hello: touch hello
## 5. Execute
* A script that adds execute permission to the owner of the file hello: chmod u+x hello
## 6. Multiple permissions
* A script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello: chmod ug+x,o+r hello
## 7. Everybody!
* A script that adds execution permission to the owner, the group owner and the other users, to the file hello: chmod ugo+x hello
## 8. James Bond
* A script that sets the permission to the file hello as follows:
   - Owner: no permission at all
   - Group: no permission at all
   - Other users: all the permissions : chmod 007 hello
## 9. John Doe
* A script that sets the mode of the file hello to this :
 -rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello
    - script = chmod 753 hello
## 10. Look in the mirror
* A script that sets the mode of the file hello the same as olleh's mode: chmod --reference=olleh hello
## 11. Directories
* A script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed: sudo chmod -R +111 */
## 12. More directories
* A script that creates a directory called dir_holberton with permissions 751 in the working directory: mkdir -m 751 dir_holberton
## 13. Change group
* A script that changes the group owner to holberton for the file hello: chgrp holberton hello
## 14. Owner and group
* A script that changes the owner to betty and the group owner to holberton for all the files and directories in the working directory: chown betty:holberton *
## 15. Symbolic links
* A script that changes the owner and the group owner of _hello to betty and holberton respectively: chown -h betty:holberton _hello
## 16. If only
* A script that changes the owner of the file hello to betty only if it is owned by the user guillaume
## 17. 