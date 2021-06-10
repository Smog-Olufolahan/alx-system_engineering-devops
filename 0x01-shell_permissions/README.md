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

   