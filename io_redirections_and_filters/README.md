README.md

Shell, I/O Redirections and filters

I/O Redirections

This feature of the command line enables you to redirect the input and/or output of commands from and/or to files, or join multiple commands together using pipes to form what is known as a “command pipeline”

1. Standard Output

2. Standard Input

3. Pipelines

4. Filters

Table of commands applied:

Questions	  Commands used

0-hello_world	  echo "Hello, World" used to display text string

1-confused_smiley echo "\"(Ôo)'" command used to display confused smiley

2-hellofile	  cat /etc/passwd used to display the content of /etc/passwd

3-twofiles	  cat /etc/passwd /etc/hosts used to display the contents of /etc/passwd & /etc/hosts

4-lastlines	  tail -10 /etc/passwd used to display 10 last lines of the file

5-firstlines	  head -10 /etc/passwd used to display 10 first lines of a file

6-third_line	  `head -n 3 iacta

7-file		  echo "Best School" > \\\*\\\\"'\"Best School\"\\'"\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*\:\) write a shell script that creates given file containing the text Best School starting with a new line

8-cwd_state	  ls -la > ls_cwd_content used standard output

9-duplicate_last_line	 tail -n 1 iacta >> iacta duplicates the last line

10-no_more_js		 find . -type f -name "*.js" -delete used to delete the files .js

11-directories		 `find . -type d -not -name '.'

12-newest_files		 `ls -t

13-unique		 `sort

14-findthatword		 grep -i "root" /etc/passwd used to display lines containing the pattern “root” from the file /etc/passwd

15-countthatword
(https://github.com/tizihoxha/shell/blob/main/io_redirections_and_filters/15-countthatword)
grep -c -i "bin" /etc/passwd used to display the number of lines that contain the pattern “bin” in the file /etc/passwd

16-whatsnext											grep -i "root" -A 3 /etc/passwd commands used to display lines containing the pattern “root” and 3 lines after them in the file /etc/passwd

17-hidethisword											grep -i -v "bin" /etc/passwd used to display all the lines in the file /etc/passwd that do not contain the pattern "bin"

18-letteronly											grep -i "^[a-z]" /etc/ssh/sshd_configdisplay all lines of the file /etc/ssh/sshd_config starting with a letter.include capital letters as well

19-AZ												`tr "A" "Z"

20-hiago											tr -d "cC"create a script that removes all letters c and C from input

21-reverse											rev script that reverse its input

22-users_and_homes										`cut -d ':' -f 1,6 /etc/passwd

23-empty_casks											`find . -empty

24-gifs												`find . -type f -name "*.gif"

25-acrostic|cut -c 1 | paste -s -d ''script that decodes acrostics that use the first letter of each line


26-the_biggest_fan|tail -n +2 | cut -f -1 | sort -k 1 | uniq -c | sort -rnk 1 | head -n 11 | rev | cut -d ' ' -f -1 | rev script that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests. 