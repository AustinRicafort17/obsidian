#notes #TOP 
![[hacker.gif|578]]
a shell is a program that lets you type in commands.,unlike the commonly used GUI, the unix shell is a CLI, basically instead of pointing and clicking with my key board i just type words and commands into a black screen and my pc follows my instructions .
bash is the most popular unis shell. <--- idk wtf this even means!

==why even use this?==

its faster 
makes automation possible
i imagine making a script (a combination of commands) that copies the chapter name of every chapter of a book trilogy and then pastes it into a text file.

![[filesystem.svg]]

/ is the root directory 
bin is for built in programs
data is for misc data files
users is for users' personal directories
tmp is for temporary files

most pc are like this.

/ is also a separator and also indicates that this is a directory

adding --help to a command shows how to use command or program

"man" before the command is the manual for it


==General Syntax of a Shell Command==

![[shell_command_syntax.svg]]

==wildcards==

*(asterisk) is a wildcard that represents 1 ore more characters .
in a directory containing : pyromancer.jpg cryomancer.jpg geomancer.jpg  gyromancer.jpg

   "(asterisk)mancer.jpg" would represent anyfile with mancer.jpg
 "p(asterisk)mancer.jpg" would only represent pyromancer.jpg

? is also a wildcard that represend just a single character

"?yromancer.jpg" means pyromancer.jpg and gyromancer.jpg

????mancer.jpg would represent all the files except geomancer.jpg because there are 4 ???? and the geo in geomancer is only 3 characters

==I NEED TO BE USING THESE WILDCARDS==


==COMMANDS==

whoami 
-shows the user of the pc

cd
-moves the cli into a directory
	cd ..
	-moves up one directory
	cd - 
	-goes back to previous directory

ls 
-lists the directories in my current pwd(present working directory) in the pc

pwd
-present working directory

clear -x
-clears out the terminal but can still access the previous lines with up and down keys

touch
-generates a new file
mkdir
-makes a directory

rm
-removes a file
	the "-i" option will promt me y/n? because rm deleting is permanent (no trashcan)
	 cant delete a directory unless with "-r" option

cp
-copies file



- `cp [old] [new]` copies a file.
- `mkdir [path]` creates a new directory.
- `mv [old] [new]` moves (renames) a file or directory.
- `rm [path]` removes (deletes) a file.
- `*` matches zero or more characters in a filename, so `*.txt` matches all files ending in `.txt`.
- `?` matches any single character in a filename, so `?.txt` matches `a.txt` but not `any.txt`.
- Use of the Control key may be described in many ways, including `Ctrl-X`, `Control-X`, and `^X`.
- The shell does not have a trash bin: once something is deleted, it’s really gone.
- Most files’ names are `something.extension`. The extension isn’t required, and doesn’t guarantee anything, but is normally used to indicate the type of data in the file.
- Depending on the type of work you do, you may need a more powerful text editor than Nano.