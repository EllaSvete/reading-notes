# Practice in the Terminal

## The Command Line

- The terminal is a text based interface to the system
- a command is typically the first thing you type.
- first line arg is referred to as an option
- used to modify behaviors of a command.
- after command has run the terminal is ready for another command.

- The Shell, Bash
  - the shell is part of the operating system that defines how the terminal will behave.
  - bash is the most common

## Basic Navigation

- pwd: print working directory
  - tells you what directory your working in.
- ls: list
- -l indicates long listing
  - First character indicates whether it is a normal file ( - ) or directory ( d )
  - Next 9 characters are permissions for the file or directory (we'll learn more about them in section 6).
  - The next field is the number of blocks (don't worry too much about this).
  - The next field is the owner of the file or directory (ryan in this case).
  - The next field is the group the file or directory belongs to (users in this case).
  - Following this is the file size.
  - Next up is the file modification time.
  - Finally we have the actual name of the file or directory.

- Paths
  - / is the root directory
  - absolute paths specify a location in relation to the root directory.
  - relative paths are in relation to where we currently are in the system.
  - ~ is the short cut off your home directory.
  - . is reference to your current directory
  - .. is reference to parent directory
  - cd allows you to move around

## More about Files

- Under the hood of linux everything is a file
- file is the command to use to figure out what type of a file is
- Linux is case sensitive
- sensitive about spacing
- use wueotes around the item
- \ escapes the special meaning of the next character
- if a file or firectory begins with a . it is considered to be hidden
- ls does not list hidden files
- ls -a will include hidden files

## Manual Pages

- Manual pages are a set of pages that explain every command available on your system including what they do, how to run them and what args they accept
- man is the command to look up a command
- q is to quit man pages
- man -k allows you to search a specific word

## FIle Manipulation

- mkdir to create a directory
- -p tells mkdir to make parent directories as needed
- -v allows mkdir to tell us what it's doing
- rmdir removes a directory
  - directory must be empty before removed
- touch creates a blank file
- cp copies a file or directory
- the hesitations can be to a file or directory
  - -r copy directory and all the files or directories in that.
- mv moves a files & directories
- rm -r allows us to remove a directory and everything in it.

## Cheat Sheat

- [Command Line Cheat Sheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)
