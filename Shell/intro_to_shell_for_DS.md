# Introduction to Shell for Data Science (DataCamp)  

## Table of Contents

- [Terminology](##Terminology)

## Terminology  
- *filesystem*: part of the operating system responsible for managing files and directories  
- *root* or *root directory*: very top of the filesystem (path: "/")
- *absolute path*: path that is the same no matter what, starts with "/" from topmost location within the computer  
- *relative path*: specifies a location relative to where you currently are  
- *parent directory*: the directory immediately above where you are currently located  



## Commands  

#### Basics  
* `pwd`: "print working directory," prints the directory where you are currently located  
* `whoami`: prints current "user" name  
* `ls <path>`: "listing," lists all files within the directory located at `<path>`  
  - `ls` with no argument lists the files in the current directory    
* `cd`: "change directory," move to a different directory   

#### Manipulating files and directories
* `cp <original> <duplicate>`: "copy," makes a copy of the file `<original>` and names it `<duplicate>`  
  - *Note:* if there is already a file called `<duplicate>`, this will overwrite that file
  - `cp <file1> <file2> <dir>` will copy all named files to the directory listed as the last parameter
* `mv <file1> <file2> <dir>`: "move," moves the named files to the directory listed as the last parameter  
	- `mv <old-name> <new-name>` can be used to rename files  
	- *Note:* if there is already a file called `<new-name>`, this will overwrite that file  
* `rm <file1> <file2>`: "remove," permanently deletes the named files  
* `mkdir <new_dir>`: "make directory," creates a new empty directory called `<new_dir>`   
* `rmdir <empty_dir>`: "remove directory," deletes an entire directory  
  - *Note:* the directory must be empty before it can be deleted
  
####Special Paths  
* `.`: special path that means "the directory you're currently in"  
* `..`: special path that means "the directory above the one you're currently in"  
* `~`: special path that means "your home directory"  
* `/tmp`: temporary directory, files that are only needed briefly can be stored here
	
	

####sec2



## Example Code  
- `cd ..`: moves back/up one directory  
- `cp seasonal/autumn.csv seasonal/winter.csv backup`: Copies the files `seasonal/autumn.csv` and `seasonal/winter.csv` and stores the copies in the directory called `backup`  
- `mv autumn.csv winter.csv ..`: Moves the files `seasonal/autumn.csv` and `seasonal/winter.csv` into the directory above where you are currently located  
