# Helpful Linuxiness #

#### Find the biggest files and directories ####
    du -Sh | sort -rh | head -n 15 

#### Touch all files in a directory ####
    find . -exec touch {} \+

#### Count Files in a Directory
    ls -l | wc -l

