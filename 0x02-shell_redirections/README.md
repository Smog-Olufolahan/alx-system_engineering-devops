# Shell, I/O Redirections and filters
## 0. Hello World
* A script that prints "Hello, World", followed by a new line to the standard output: echo "Hello, World"
## 1. Confused smiley
* A script that displays a confused smiley: echo \"\(Oo\)\"
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
* A script that creates a file named exactly \*\\'"Holberton School"\'\\*$\?\*\*\*\*\*:) containing the text Holberton School ending by a new line: echo "Holberton School" | cat > '\*\\'\''"Holberton School"\'\''\\*$\*\*\*\*\*:)
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
* A script that takes a list of words as input and prints only words that appear exactly once: 