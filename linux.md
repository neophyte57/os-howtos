# Check hash value of file 

`sha256sum afile.bin`


# Check what is running on a TCP port 

Try `lsof` (e.g. `lsof -i:4200`) or `netstat` (e.g. `sudo netstat -plnt | grep ':80'`).  Regarding the latter, for more info:  https://support.rackspace.com/how-to/checking-listening-ports-with-netstat/ 


# Clear console

`clear`, roughly equivalent to Windows `cls`


# Copy files between machines using ssh

`scp <path to file> <user id>@<destination address>:<destination path>`, e.g. To copy an archive to the home directory of the user `neophyte` on another computer:  `scp .\dags.7z neophyte@192.168.1.65:~`


# Find files by file content  

`grep -Ri "text-to-find-here" .`.  For more info, see:  <https://stackoverflow.com/questions/16956810/how-do-i-find-all-files-containing-specific-text-on-linux> 


# Find files by filename 

`find /path/to/folder/ -iname *file_name_portion*`.  Use `-name` for case-sensitive search.


# Saving history of commands 

If the commands typed into the console are very precious, save history periodically with `history -a`.  For more information:  https://askubuntu.com/questions/885531/half-of-bash-history-is-missing


# View IP address

`ip addr show`
