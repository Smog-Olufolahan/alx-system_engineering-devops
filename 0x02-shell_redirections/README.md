# Shell, I/O Redirections and filters
## 0. Hello World
* A script that prints "Hello, World", followed by a new line to the standard output: echo "Hello, World"
## 1. Confused smiley
* A script that displays a confused smiley: echo "\"(Ôo\)\'"
## 2. Let's display a file
* Display the content of the /etc/passwd file: cat /etc/passwd
## 3. What about 2?
* Display the content of /etc/passwd and /etc/hosts: cat /etc/passwd /etc/hosts
## 4. Last lines of a file
* Display the last 10 lines of /etc/passwd: tail -n 10 /etc/passwd
## 5. I'd prefer the first ones actually
* Display the first 10 lines of /etc/passwd: head -n 10 /etc/passwd
## 6. Line #2
* A script that display the third line of the file iacta: head -n 3 iacta | tail -n 1
## 7. It is a good file that cuts iron without making a noise
* A script that creates a file named exactly \*\\'"Holberton School"\'\\*$\?\*\*\*\*\*:) containing the text Holberton School ending by a new line: echo "Holberton School" | cat > '\*\\'\''"Holberton School"\'\''\\*$\*\*\*\*\*:)'
## 8. Save current state of directory
* A script that writes into the file ls_cwd_content the result of the command ls -la: ls -la > ls_cwd_content
## 9. Duplicate last line
* A script that duplicates the last line of the file iacta: tail -n 1 iacta | cat >> iacta
## 10. No more javascript
* A script that deletes all the regular files(not the directories) with a .js extension that are present in the current directory and all its subfolders: find . -name "*.js" -type f -delete
## 11. Don't just your directories, make your directories count
* A script that counts the number of directories and sub-directories in the current directory: find . -mindepth 1 -type d | wc -l
## 12. What's new
* A script that displays the 10 newest files in the current directory: ls -t | head
## 13. Being unique is better than being perfect
* A script that takes a list of words as input and prints only words that appear exactly once: sort | uniq -u
## 14. It must be in that file
* A script that display lines containing the pattern "root" from the file /etc/passwd: grep root /etc/passwd
## 15. Count that word
* A script that display the number of lines that pattern "bin" in the file /etc/passwd: grep -c bin /etc/passwd
## 16. What's next
* A script that display lines containing the pattern "root" and 3 lines after them in the file /etc/passwd: cat /etc/passwd | grep -A 3 "root"
## 17. I hate bins
*A script that display all the lines in the file /etc/passwd that do not contain the pattern "bin": grep -v bin /etc/passwd
## 18. Letters only please
* A script that display all lines of the file /etc/ssh/sshd_config starting with a letter: grep ^[[:alpha:]] /etc/ssh/sshd_config
## 19. A to Z
* A script to replace all xters A and c from input to Z and e respectively: tr 'Ac' 'Ze'
## 20. Without C, you will live in hiago
* A script that removes all letters c and C from input: tr -d 'Cc'
## 21. esreveR
* A script that reverse its input: rev
## 22. DJ Cut Killer
* A script that displays all users and their home directories, sorted by users: cut -d":" --fields=1,6 /etc/passwd | sort
## 23. Empty casks make the most noise
* A script that finds all empty files and directories in the current directory and all sub-directories: find . -empty -printf "%f\n"
## 24. A gif is worth ten thousand words
* A script that lists all the files with a .gif extension in the current directory and all its sub_directories: *.gif check repo for answer.
## 25. Acrostic
*A script that decodes acrostics that use the first letter of each line: echo -ne $(cut -c-1 | tr -d '\n')'\n'
## 26. The biggest fan
* A script that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests: tail -n +2 | cut -f1 | sort | uniq -c | sort -nr -k 1,1 | cut -c 9- | head -11
