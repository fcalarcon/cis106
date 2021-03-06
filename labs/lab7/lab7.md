---
name: Fiorella Alarcon
---

# date

## Description
displays date and time

## Syntax
`date`

## Example
* display current date and time:
  * `date`


# uname

## Description
displays information about your system

## Syntax
`uname`

## Example
*display  system information
`uname`

# free

## Description
displays the amount of free memory

## Syntax
`free`

## Example
display free memory
`free`

## pwd

## Description
used for displaying the current working directory

## Syntax
`pwd`

## Example 
* display current directory
  * `pwd`   

## cd

## Description
used for changing the current working directory. When no directory is given, cd changes the working directory to the home director of the current user.

## Syntax
`cd + destination`

## Examples
* go to home directory
  * `cd`
* go to previous current working directory
  * `cd -`
* goback 1 or ore directories
  * `cd ../`


# ls

## Description
used for displaying all the files inside a given directory. When no directory is specified, ls displays the files in the current working directory

## syntax
`ls + option + argument`

## Examples
* list all the files inside the current working directory including hidden files
  * `ls -a`
* list all the files inside a given directory
  * `ls -a ~/Pictures`
* list all the files in a given directory sorted by last modified
  * `ls -t ~/Documents`


# mkdir

## Description
It is used for creating directories

## Syntax
`mkdir + option + directories to make`

## Examples
* Make a directory
  * `mkdir newDirectory`
* Make 2 directories
  * `mkdir newDirectory NewDirectory2`
* Make a parent and child directory
  * `mkdir -p Pets/Dogs/`

# touch

## Description
used for creating files

## Syntax
`touch + file_name`

## Examples
* to create a file called list
  * `touch list`
* to create several files
  * `touch stars.txt script.py`
* to create a file with a space in its name`
  * `touch "hearts and stars.txt"`
  
# rm

## Description
removes files.

## Syntax
`rm + option + file name`

## Examples
* remove a file
  * `rm list`
* remove an non-empty directory
  * `rm -r Downloads/fun`
* remove a file and prompt confirmation before removal 
  * `rm -i list`

# cp

## Description 
cp copies files/directories from a source to a destination

## Syntax
`cp + files to copy + destination`
`cp -r + directory to copy + destination`

## Examples
* copy a file
  * `cp Downloads/wallpapers.zip Pictures/`
* copy multiple files
  * `sudo cp -r script.s program.py`
* copy the content of a drectory to another directory
  * `cp Downloads/wallpapers/* ~/Pictures/`

# mv

## Description
moves and renames directories

## Syntax
`mv + source + destination`
`mv + file/directory to rename + new name`

## Examples
* to move a file froma directory to another 
  * `mv Downloads/hw.pdf Documents/`
* to rename a file
  * `mv hw.docx hw1.docx`
* to move and rename a file in the same command
  * `Downloads/hw.docx Documents/classes.docx`


stat
# Wildcards (*,?,[])

## Description
* (*) matches anything and nothing and matches any number of characters
* ? matches precisely one character
* [] match a single character in a range 

## Syntax
* `ls + (*,?,[])`

## Examples
* match all files tha en in .txt
  * `ls *.txt`
* list all hidden files
  * `ls .??*`
* match all files that have a vowel after letter f
  * `ls f[!aeiou]*`

# Brace expansion

# Description
feature of bash allows you to generate arbitrary strings to use with commands

## Syntax
`command + option + file name`

## Examples
* to create a N number of files
  * `touch website{1..5}.html`

# cat

## Description
used for displaying the content of a file

## Syntax
`cat + option + files(s) to display`

## Example
* display content of a file located in the pwd
  * `cat todo.md`

## head

## Description
displays the op N number of lines of a given file

## Syntax
`head + option + file(s)`

## Example
* display the first 10 lines of a file
  * `head ~/Documents/Book/dracula.txt`
  
# tail 

## Description
displays the last N number of lines of a given file

## Syntax 
`tail + option + file`

## Example
* display the last 10 lines of a file
  * `tail ~/Documents?Book/Dracula.txt`

# cut

## Description
used to exact a specific section of each line of a file and display it to the screen

## Syntax
`cut + option + file(s)`

## Example
* `cut -d ':' -f1 /etc/passwd`

# tr

## Description
translating or deleting characters from standard output

## Syntax
`tr + option +set +set`

## Example
* translate one character to another 
  * `cat file.txt | '.' ','`


# paste

## Description
joining files horizontally in columns

## Syntax
`paste + option + files`

## Example
* merge two files
  * `paste users.1st ip_address.1st`

# wc

## Description
printing the number of lines, characters and bytes in a file

## Syntax
`wc + option file(s)`

## example
* display the number of lines in a file
  * `wc -l users.txt`

# grep

## Description
to search tex in given file

## Syntax
`grep + option + search criteria + file(s)

## Example
* search any line that contais the word "dracula" in the given file
  * `grep 'dracula' ~/Documents/dracula.txt`

