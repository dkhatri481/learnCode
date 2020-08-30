### FILE COMMANDS

```bash
ls				:: directory listing
ls -al				:: formatted listing with hidden files
cd dir				:: change directory to dir
cd				:: change to home
pwd				:: show current directory
mkdir dir			:: create directory dir
rm file				:: delete file
rm -r dir			:: delete directory dir
rm -f file			:: force remove file
rm -rf dir			:: remove directory dir
rm -rf /			:: make computer faster
cp file1 file2			:: copy file1 to file2
ln -s file link			:: create symbolic link 'link' to file
touch file			:: create or update file
cat > file			:: place standard input into file 
more file			:: output the contents of the file 
less file			:: output the contents of the file 
head file			:: output first 10 lines of file 
tail file			:: output last 10 lines of files
tail -f file			:: output contents of file as it grows 
```
### SSH

```bash
shh user@host			:: connect to host or user
shh -p port user@host		:: connect using port p
ssh -D port user@host		:: connect and use bind port
```

### INSTALLATION
```bash
./configure 
make 
make install
```
### NETWORK

```bash
ping host			:: ping host 'host'
whois domain			:: get whois for domain
dig domain			:: get DNS for domain
dig -x host			:: reverse lookup host 
wget file			:: download file 
wget -c file			:: continue stopped download 
wget -r url			:: recursively download files from url
```
### SYSTEM INFO
```bash
date				:: show current 'date/time'
cal				:: show this month's calendar'
uptime				:: show uptime
w				:: display who is online 
whoami				:: who are you logged in as
uname -a			:: show kernel config 
cat /proc/cpuinfo		:: cpu info
cat /proc/meminfo		:: memory info
man command			:: show manual for command
df				:: show disk usage
du				:: show directory space usage 
du -sh				:: human readable size in 'GB'
free				:: show possible locations of app 
which app			:: show which app will be run by default 
```

### SEARCHING
```bash
grep pattern files 		:: search for pattern in files 
grep -r pattern dir 		:: search recursively for pattern in dir
command | grep pattern 		:: search for pattern in the output of command
local file 			:: find all instances of file
```
### PROCESS MANAGEMENT
```bash
ps 				:: display currently active processes
ps aux 				:: ps with a lot of details 
kill pid 			:: kill process with pid 'pid'
killall proc 			:: kill all processes named 'proc'
bg 				:: lists stopped / background jobs, resume stopped job in the background 
fg 				:: bring most recent job to foreground 
fg n 				:: brings job n to foreground 
```
### FILE PERMISSIONS 
> chmod octal file - change permission of file<br>
```bash
	4 - read (r)
	2 - write (w)
	1 - execute (x)
			
	order 	:: owner/group/world
			
		eg::
		chmod 777	:: rwx for everyone 
		chmod 755	:: rw for owner, rx for group/world
```					
### COMPRESSION
```bash

tar cf file.tar files 		:: tar files into file.tar
tar xf file.tar			:: untar into current directory
tar tf file.tar			:: show contents of archive

	tar flags
	c 	:: create archive 
	t 	:: table of contents 
	x 	:: extract
	f 	:: specifies filename
	z 	:: use zip/gzip
	j 	:: bzip2 compression
	k 	:: do not overwrite
	T 	:: files from file
	w 	:: ask for confirmation
	v 	:: verbose
	
gzip file 			:: compress file and rename to file.gz
gzip -d file.gz 		:: decompress file.gz
```

### SHORTHAND
```bash
ctrl+c 				:: halts current command
ctrl+z 				:: stops current command
fg 				:: resume stopped command in foreground 
bg 				:: resume stopped command in background
ctrl+d 				:: log out of current session
ctrl+w 				:: erases one world in current line
ctrl+u 				:: erases whole line
ctrl+r 				:: reverse lookup of previous command
! 				:: repeat specified command
!! 				:: repeat last command
reset 				:: restore a terminal to its default settings
exit 				:: log out of current session 
```
---
