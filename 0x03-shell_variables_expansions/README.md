# Shell, init files, variables and expansions
## 0. <0>
* A script that creates an alias: alias ls="rm *"
## 1. Hello you
* A script that prints hello user, where user is the current Linux user: echo "hello $USER"
## 2. The path to success is to take massive, determined action
* A script that add /action to the PATH. /action should be the last directory the shell looks into when looking for a program: PATH=$PATH:/action
## 3. If the path be beautiful, let us not ask where it leads
* A script that counts the number of directories in the PATH: echo $PATH | tr ":" "\n" | wc -l
## 4. Global variables
* A script that lists environment variables: printenv
## 5. Local variables
* A script that lists all local variables and environment variables, and functions: set
## 6. Local variable
* A script that creates a new local variable: BETTY=Holberton
  - Name: BETTY
  - Value: Holberton
## 7. Global variable  
* A script that creates a new global variable: export HOLBERTON=Betty
## 8. Every addition to true knowledge is an addition to human power
* A script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line: echo $(($TRUEKNOWLEDGE+128))
