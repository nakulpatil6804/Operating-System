# Operating-System
PRACTICAL NO: 1
Definition: Study of Basic commands of Linux/UNIX.
Command shell: A program that interprets commands is Command shell.
Shell Script: Allows a user to execute commands by typing them manually at a terminal, or
automatically in programs called shell scripts.
A shell is not an operating system. It is a way to interface with the operating system and run
Commands.
BASH (Bourne Again Shell)
• Bash is a shell written as a free replacement to the standard Bourne Shell (/bin/sh) originally
written by Steve Bourne for UNIX systems.
• It has all of the features of the original Bourne Shell, plus additions that make it easier to
program with and use from the command line.
• Since it is Free Software, it has been adopted as the default shell on most Linux systems.
BASIC LINUX COMMANDS:
1. pwd : Print Working Directory
DESCRIPTION:
pwd prints the full pathname of the current working directory.
SYNTAX:
pwd
EXAMPLE:
$ pwd
/home/directory_name
2. cd: Change Directory
DESCRIPTION:
It allows you to change your working directory. You use it to move around within
the hierarchy of your file system.
SYNTAX:
cd directory_name
EXAMPLE:
To change into “work directory” in “documents” need to write as follows.
Input: $ cd /documents/work
3. cd ..
DESCRIPTION:
Move up one directory.
SYNTAX:
cd ..
EXAMPLE:
If you are in work directory and want to go to documents then write
cd ..
You will end up in /documents.
4. ls : list all the files and directories
DESCRIPTION:
List all files and folders in the current directory in the column format.
SYNTAX:
ls [options]
EXAMPLE: Using various options
• Lists the total files in the directory and subdirectories, the names of the files in the current
directory, their permissions, the number of subdirectories in directories listed, the size of the
file, and the date of last modification.
ls -l
• List all files including hidden files
ls -a
5. cat
DESCRIPTION:
cat stands for "catenate". It reads data from files, and outputs their contents. It is the simplest
way to display the contents of a file at the command line.
SYNTAX:
cat filename
EXAMPLES:
• Print the contents of files mytext.txt and yourtext.txt
cat mytext.txt yourtext.txt
• Print the cpu information using cat command
cat /proc/cpuinfo
• Print the memory information using cat command
cat /proc/meminfo
6. head
DESCRIPTION:
head, by default, prints the first 10 lines of each FILE to standard output. With more than one
FILE, it precedes each set of output with a header identifying the file name.
If no FILE is specified, or when FILE is specified as a dash ("-"), head reads from standard input.
SYNTAX:
head [option]…[file/directory]
EXAMPLE:
Display the first ten lines of myfile.txt.
head myfile.txt
7. tail
8. DESCRIPTION:
tail is a command which prints the last few number of lines (10 lines by default) of a certain
file, then terminates.
SYNTAX:
tail [option]…[file/directory]
EXAMPLE:
Output the last 100 lines of the file myfile.txt.
tail myfile.txt -n 100
8. mv : Moving (and Renaming) Files
DESCRIPTION:
The mv command lets you move a file from one directory location to another. It also lets you
rename a file (there is no separate rename command).
SYNTAX:
mv [option] source directory
EXAMPLE:
• Moves the file myfile.txt to the directory destination-directory.
mv myfile.txt destination_directory
• Move the file myfile.txt into the parent directory.
mv myfile.txt ../
• In this case, if JOE1_expenses does not exist, it will be created with the exact content
ofjoe_expenses, and joe_expenses will disappear.
If JOE1_expenses already exists, its content will be replaced with that
of joe_expenses (and joe_expenses will still disappear).
mv joe_expenses JOE1_expenses
9. mkdir : Make Directory
DESCRIPTION:
If the specified directory does not already exist, mkdir creates it. More than one directory
may be specified when calling mkdir.
SYNTAX:
mkdir [option] directory
EXAMPLE:
Create a directory named work.
mkdir work
10. cp : Copy Files
DESCRIPTION:
The cp command is used to make copy of files and directories.
SYNTAX:
cp [option] source directory
EXAMPLE:
Creates a copy of the file in the currently working directory named origfile. The copy will be
named newfile, and will be located in the working directory.
cp origfile newfile
11. rmdir : Romove Directory
DESCRIPTION:
The rmdir command is used to remove a directory that contains other files or directories.
SYNTAX:
rm directory_name
EXAMPLE:
Delete mydir directory along with all files and directories within that directory. Here, -r is for
recursive and –f is for forcefully
rmdir -rf mydir
12. gedit
DESCRIPTION:
The gedit command is used to create and open a file.
SYNTAX:
gedit filename.txt
EXAMPLE:
To create a file named abc.sh
gedit abc.sh
13. man
DESCRIPTION:
Displays on online manual page or manpage.
SYNTAX:
man command
EXAMPLE:
To learn about listing files
man ls
14. echo
DESCRIPTION:
Display text on the screen.
SYNTAX:
echo yourtext
EXAMPLE:
Print Hello World on the screen
echo “Hello World”
15. clear
DESCRIPTION:
Used to clear the screen
SYNTAX:
clear
EXAMPLE:
Clear the entire screen
clear
16. whoami
DESCRIPTION:
whoami prints the effective user ID. This command prints the username associated with the
current effective user ID.
SYNTAX:
whoami [option]
EXAMPLE:
Display the name of the user who runs the command.
whoami
17. wc
DESCRIPTION:
wc (word count) command, can return the number of lines, words, and characters in a file.
SYNTAX:
wc [option]… [file]…
EXAMPLE:
• Print the byte counts of file myfile.txt
wc -c myfile.txt
• Print the line counts of file myfile.txt
wc -l myfile.txt
• Print the word counts of file myfile.txt
wc -w myfile.txt
18. grep
DESCRIPTION:
grep command uses a search term to look through a file.
SYNTAX:
grep [option]… Pattern [file]…
EXAMPLE:
Search the word Hello in file named myfile.txt
grep “Hello” myfile.txt
19. free
DESCRIPTION:
Display RAM details in Linux machine.
SYNTAX:
free
EXAMPLE:
To display the RAM details in Linux machine need to write following command.
free
20. pipe ( | )
DESCRIPTION:
Pipe command is used to send output of one program as a input to another. Pipes “|” help
combine 2 or more commands.
SYNTAX:
Command 1 | command 2
EXAMPLE:
Display lines of input files containing “Aug” and send to standard output
ls -l | grep “Aug”
