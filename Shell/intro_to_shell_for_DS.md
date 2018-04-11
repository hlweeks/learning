# Introduction to Shell for Data Science  
## DataCamp Course  

### Commands  

#### Manipulating Files and Directories
* `pwd`: "print working directory," prints the directory where you are currently located  
* `whoami`: prints current "user" name  
* `ls`: "listing," lists all files and directories within the current directory. Alternatively, typing `ls HOME/DIRECTORY` will show all files listed within the folder called "DIRECTORY"  
* `cd`: "change directory," move to a different directory  
* `.`: special path that means "the directory you're currently in"  
* `..`: special path that means "the directory above the one you're currently in"  
* `~`: special path that means "your home directory"  
* `cp <original> <duplicate>`: "copy," makes a copy of the file `<original>` and names it `<duplicate>`  
  - *Note:* if there is already a file called `<duplicate>`, this will overwrite that file
  - `cp <file1> <file2> <dir>` will copy all named files to the directory listed as the last parameter
* `mv <file1> <file2> <dir>`: "move," moves the named files to the directory listed as the last parameter  
	- `mv <old-name> <new-name>` can be used to rename files  
	- *Note:* if there is already a file called `<new-name>`, this will overwrite that file  
	
	

####sec2



### Terminology  
- *filesystem*: **insert**
- *root directory*: very top of the filesystem (path: "/")
- *absolute path*: path that is the same no matter what, starts with "/" from topmost location within the computer  
- *relative path*: specifies a location relative to where you currently are  
- *parent directory*: the directory immediately above where you are currently located  


### Example Code  
- `cd ..`: moves back/up one directory  
- `cp seasonal/autumn.csv seasonal/winter.csv backup`: Copies the files `seasonal/autumn.csv` and `seasonal/winter.csv` and stores the copies in the directory called `backup`  
- `mv autumn.csv winter.csv ..`: Moves the files `seasonal/autumn.csv` and `seasonal/winter.csv` into the directory above where you are currently located  
