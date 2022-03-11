### Linux Tutorial Cheatsheet 1-3 ###
###### The Command Line
- The command line is also known as the terminal 
  - It is a text based interface to the system. You can give commands, and feedback will be given as you enter them. 
- Line 1
  - presents us with a prompt
   - we enter command - first thing you type. 
   - then, we have command line arugments. There must be a space between the command and the first command line argument. 
   - First command argument (-l) is also refered to as an option. 
   - Options modify behaviors of the command. 
   - Options are usually listed before other arguments and typically start with a dash ( - ).
- Line 2-5 
   - Outputs for running commands. 
- Line 6 
   - Prompt again
###### Opening a Terminal
- Termial > applications > utilities or command + space
- The shell is part of the operating system that defines how the terminal will behave and look after you give it commands. 
- Bash refers to a shell
- To know which shell you are using, use echo $shell 
###### Shortcuts
When you enter commands, they are a history. You can traverse this history using the up and down arrow keys. So don't bother re-typing out commands you have previously entered, you can usually just hit the up arrow a few times. You can also edit these commands using the left and right arrow keys to move the cursor where you want.

###### Basic Navigation
- pwd > Print Working Directory
  - Use this command to remind yourself where you are in the terminal
- ls > list 
  - With no arguments it will give a plain listing of current location 
  - ls[option][location] > square brackets mean items are optional > we can run command with or without them
  - (/etc.) tells ls to not list our current directories but list it's contents.
- Path > refers to a file or directory on the command line 
- There are 2 types of paths: *absolute* and and *relative*
- The top is called the *root* directory and is denoted by a slash (/)
  - This slash is how you can identitify absolute paths in relation to the directory
  - relatvie paths will not begin with a slash. They specify a specific location 
- ~ (tilde) > shortcut for home directory 
- . (dot) > reference to your current directory
- .. (dotdot) > reference to parent directory
- cd > stands for change directory

###### More About Files!
- Common Extensions > 
  - file.exe - an executable file, or program.
  - file.txt - a plain text file.
  - file.png, file.gif, file.jpg - an image.
- You can use the command file to find out what the file is 
-  whenever we specify a file or directory on the command line it is actually a path file[path]
-  Linux is case sensitive!
-  Command lines are also case sensitive
-  Don't have a space in file names unless it has quotes 'Holiday Photos' or \Holiday Photos
-  . (full stop) means the file is hidden > to hide a file you can have it begin with a . 
-  ls will not list hidden files
