# Helpful Linuxiness #


#### Find the biggest files and directories ####

    du -Sh | sort -rh | head -n 15 
[http://ask.xmodulo.com/find-biggest-files-directories-linux.html](http://ask.xmodulo.com/find-biggest-files-directories-linux.html "Source")

#### Touch all files in a directory ####
    find . -exec touch {} \+
[http://unix.stackexchange.com/questions/22291/touch-all-folders-in-a-directory](http://unix.stackexchange.com/questions/22291/touch-all-folders-in-a-directory)

#### Count Files in a Directory
    ls -l | wc -l

#### Get total directory size
    du -hs /path/to/directory
[http://askubuntu.com/questions/1224/how-do-i-determine-the-total-size-of-a-directory-folder-from-the-command-line](http://askubuntu.com/questions/1224/how-do-i-determine-the-total-size-of-a-directory-folder-from-the-command-line)

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

#### Find Installed RPM
	rpm -qa |grep -i <rpm>
Note: The -i on grep will ignore case

#### Get RPM scripts
	rpm -qp --scripts MySQL-server-5.6.23-1.el6.i686.rpm > /tmp/scripts
From: [http://help.lockergnome.com/linux/extract-pre-post-scripts-binary-rpm--ftopict418302.html](http://help.lockergnome.com/linux/extract-pre-post-scripts-binary-rpm--ftopict418302.html "http://help.lockergnome.com/linux/extract-pre-post-scripts-binary-rpm--ftopict418302.html")

#### Bash Comparison Operators
	-gt
[http://tldp.org/LDP/abs/html/comparison-ops.html](http://tldp.org/LDP/abs/html/comparison-ops.html)

#### Extracting Files from RPM
	mkdir rpm
	cd rpm
	<place rpm to extract here>
	rpm2cpio <rpm-name> | cpio -idmv
From: [http://www.cyberciti.biz/tips/how-to-extract-an-rpm-package-without-installing-it.html](http://www.cyberciti.biz/tips/how-to-extract-an-rpm-package-without-installing-it.html "Extract RPM Files")
