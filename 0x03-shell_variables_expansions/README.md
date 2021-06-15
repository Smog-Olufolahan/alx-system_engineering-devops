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
## 9. Divide and rule
* A script that prints the result of POWER divided by DIVIDE, followed by a new line: echo $(($POWER/DIVIDE))
## 10. Love is another to life, posterior to death, initial of creation, and the exponent of breath
* A script that display the result of BREATH to the power LOVE: echo $(($BREATH**$LOVE))
## 11. There are 10 types of people in the world -- Those who understand binary, and those who don't
* A script that converts a number from base 2 to base 10: echo $((2#$BINARY))
## 12. Combination
* A script that prints all possible combinations of two letters, expect oo: echo {a..z}{a..z} | tr ' ' '\n' | grep -v oo
## 13. Floats
* A script that prints a number with two decimal places, followed by a new line: printf "%0.2f\n" $NUM
## 14. Decimal to Hexadecimal
* A script that converts a number from base 10 to base 16: prinf "%x\n" $DECIMAL
## 15. Everyone is a proponent of strong encryption
* A script that encodes and decodes text using the root13 encryption. Assume ASCII: tr 'A-Za-z' 'N-ZA-Mn-za-m'
## 16. The eggs of the brood need to be an odd number
* A script that prints every other line from the input, starting with the first line: paste -d" " - - | cut -d " " -f 1
## 17. I'm an instant star. Just add water and stir
* A script that adds the two numbers stored in the environment variables WATER and STIR and prints the result : printf '%o\n'
