## Basic commands
```
🔸 cd /directory              moves the present working directory to one specified
🔸 cp /copied_item /target    copies a filed or directory to a target directory. If your copying a directory use cp -rf . .
🔸 pwd                        shows the absolute path of where you are (present working directory)
🔸 chmod ### file             how you give or remove access to files. first digit is you, second is group and last is all users 
(read=4,write=2,execute=1. ex: use 777 for full access to everyone)
🔸 diff /file /file           outputs the lines that do not match between the two files
🔸 rm file                    remove command lets you remove a file. Removing a directory requires -rf (ex: rm -rf dir)
🔸 mkdir directoryname        makes a directory with the name specified
🔸 touch filename             makes a file with the name specified
🔸 mv file file               lets you move a file somewhere else and is also used to rename files
🔸 cat file                   displays the text of a file
🔸 man "command"              displays the manual for the command specified. Useful to find options for the command quickly
🔸 history                    shows the commands you've entered
🔸 ctrl+c                     quits you out of most programs
🔸 |                          this symbol is called "pipe" and is used to feed output of one command into another command without 
storing it into a variable (ex: "ls -s | head -5" takes the list of files ordered by size from ls and prints the top 5 of them)

```
## ls
**ls commands** ``` $ ls [options] [file|dir] ```
```
🔸 ls -a          list all files including hidden file starting with '.'
🔸 ls --color     colored list [=always/never/auto]
🔸 ls -d          list directories
🔸 ls -i          list file's inode index number
🔸 ls -l          list with long format - show permissions
🔸 ls -la         list long format including hidden files
🔸 ls -lh         list long format with readable file size
🔸 ls -ls         list with long format with file size
🔸 ls -r          list in reverse order
🔸 ls -R          list recursively directory tree
🔸 ls -s          list file size
🔸 ls -S          sort by file size
🔸 ls -t          sort by time & date
🔸 ls -X          sort by extension name
```
## grep
**grep commands** ``` grep [options] pattern [files] ```
```
🔸 grep -c        This prints only a count of the lines that match a pattern
🔸 grep -h        Display the matched lines, but do not display the filenames
🔸 grep -i        Ignores, case for matching
🔸 grep -l        Displays list of a filenames only
🔸 grep -n        Display the matched lines and their line numbers.
🔸 grep -v        This prints out all the lines that do not matches the pattern
🔸 grep -e exp    Specifies expression with this option. Can use multiple times
🔸 grep -f file   Takes patterns from file, one per line
🔸 grep -E        Treats pattern as an extended regular expression (ERE)
🔸 grep -w        Match whole word      
```
## sed
**sed commands** ``` sed [option] 'command' [input-file] ```
```
🔸 sed '/^$/d'    Remove all whitespace
🔸 sed 's/Sonday/Sunday/' weekday.txt
🔸 sed -i         When option, edit source file directly. Also used to ignore case when flag
🔸 sed -g         Edit every occurence
🔸 ^              Acts like a special character and matches at the beginning of the regular exp
🔸 $              Acts like a special character and matches at the end of the regular exp 
🔸 .              Matches any single character, even including a new line
🔸 *              Matches the sequence of zero or more instances of the previous character
🔸 sed 's/Linux/Unix/'  linuxteck.txt (first occurence in each line)
🔸 sed 's/Linux/Unix/2' linuxteck.txt (Second occurence in each line)
```
## sort
**sort commands** ``` sort [OPTION]... [FILE]... ```
```
🔸 sort -b        Remove all whitespace
🔸 sort -d        Consider only blanks and alphanumeric characters
🔸 sort -f        Fold lower case to upper case characters
🔸 sort -g        Compare according to general numerical value
🔸 sort -i        Consider only printable characters
🔸 sort -n        Compare according to string numerical value
```
## head/tail
**head commands** ``` head [OPTION]... [FILE]... ```
```
🔸 head -n #      Print number of lines from top down
🔸 tail -#        prints last # of elements (lines/files)
```
