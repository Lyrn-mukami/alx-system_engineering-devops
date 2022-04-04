0.Hello World
Write a script that prints “Hello, World”, followed by a new line to the standard output.
	echo "Hello, World\n"
1.Confused smiley
Write a script that displays a confused smiley "(Ôo)'.
echo -e "\U0001f615"
2.Let's display a file
Display the content of the /etc/passwd file.
cat /etc/passwd
3.What about 2?
Display the content of /etc/passwd and /etc/hosts
cat /etc/passwd /etc/hosts
4.Last lines of a file
Display the last 10 lines of /etc/passwd
tail /etc/passwd (tail by default displays the last 10 lines of a file)
5.I'd prefer the first ones actually
Display the first 10 lines of /etc/passwd
head /etc/passwd
6.Lines #2
Write a script that displays the third line of the file iacta
The file iacta will be in the working directory
You’re not allowed to use sed
head -n 4 iacta
7.It is a good file that cuts iron without making a noise
Write a shell script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line.
echo "Best School" >  \*\\'"Best School"\'\\*$\?\*\*\*\*\*:)
8.Save current state of directory
Write a script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it.
ls -la >ls_cwd_content
9.Duplicate last line 
Write a script that duplicates the last line of the file iacta
last -1 iacta >> iacta
10.no more javascript
Write a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders.
find . -name *.js -delete
11.Don't just count your directories, make your directories count
Write a script that counts the number of directories and sub-directories in the current directory.
find /0x02-shell_redirections -type p |wc -l
12.What's new
Create a script that displays the 10 newest files in the current directory.
ls -1t |head -10
13.Create a script that takes a list of words as input and prints only words that appear exactly once.
cat list |uniq | sort | tr '\n'
14.IT must be in that file
Display lines containing the pattern “root” from the file /etc/passwd
grep root /etc/passwd
15.Count that word
Display the number of lines that contain the pattern “bin” in the file /etc/passwd
grep -c bin etc/passwd
16.What's next?
Display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd
grep -A 3 "root" /etc/passwd
17.I hate bins
Display all the lines in the file /etc/passwd that do not contain the pattern “bin”.
grep -v "bin" /etc/passwd
18.Letters only please
Display all lines of the file /etc/ssh/sshd_config starting with a letter.
grep '[a-zA-Z]' /etc/ssh/sshd_config
19.A to Z
Replace all characters A and c from input to Z and e respectively.
echo 'Replace all characters `A` and `c` from input to `Z` and `e`.' | tr 'Ac' 'Ze'
20.Without C, you would live in hiago
Create a script that removes all letters c and C from input.
echo Chicago | tr -d 'cC'
21.esreveR
Write a script that reverse its input.
 echo "Reverse" | rev
