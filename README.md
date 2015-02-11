# Helpful Linuxiness #

#### Find the biggest files and directories ####
    du -Sh | sort -rh | head -n 15 
[http://ask.xmodulo.com/find-biggest-files-directories-linux.html](http://ask.xmodulo.com/find-biggest-files-directories-linux.html "Source")

#### Touch all files in a directory ####
    find . -exec touch {} \+
[http://unix.stackexchange.com/questions/22291/touch-all-folders-in-a-directory](http://unix.stackexchange.com/questions/22291/touch-all-folders-in-a-directory)

#### Count Files in a Directory
    ls -l | wc -l

#### chmod Number Codes 
    0 == --- == no access
	1 == --x == execute
	2 == -w- == write
	3 == -wx == write / execute
	4 == r-- == read
	5 == r-x == read / execute
	6 == rw- == read / write
	7 == rwx == read / write / execute

#### Adding alias's to bashrc
	vi ~/.bashrc
	
		alias ll='ls-al'
		:wq

	source ~/.bashrc